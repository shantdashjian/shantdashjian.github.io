---
title: "Continuous Deployment" # Title of the blog post.
date: 2023-07-20T10:38:49+04:00 # Date of post creation.
tags:
  - continuous deployment
  - github actions
  - devops
  - yaml
# comment: false # Disable comment if false.
---

Yesterday I explored using GitHub Actions workflows for continuous deployment. I used a pipeline that takes code 
pushed to GitHub all the way to production, deployed on a Kubernetes cluster on Azure cloud. 

The deployment workflow is written in YAML, and in it there 4 levels:
- workflow
  - jobs
    - steps
      - commands

Here is an example workflow, from Chapter 8 of the book [Bootstrapping Microservices, by Ashley Davis](https://www.manning.com/books/bootstrapping-microservices-second-edition).
```
name: Deploy microservice

on:
  push: 
    branches:
      - main
  workflow_dispatch: 

jobs:

  deploy:
    runs-on: ubuntu-latest
    
    env:
      VERSION: ${{ github.sha }}
      CONTAINER_REGISTRY: ${{ secrets.CONTAINER_REGISTRY }}
      REGISTRY_UN: ${{ secrets.REGISTRY_UN }}
      REGISTRY_PW: ${{ secrets.REGISTRY_PW  }}

    steps:
      
      - uses: actions/checkout@v3

      - name: Build
        run: ./scripts/build-image.sh

      - name: Publish
        run: ./scripts/push-image.sh

      - uses: tale/kubectl-action@v1
        with:
          base64-kube-config: ${{ secrets.KUBE_CONFIG }}
          kubectl-version: v1.26.0
      
      - name: Deploy
        run: ./scripts/deploy.sh
```


