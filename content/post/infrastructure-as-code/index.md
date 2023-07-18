---
title: "Infrastructure as Code" # Title of the blog post.
date: 2023-07-18T10:14:20+04:00 # Date of post creation.
tags:
  - infrastructure as code
  - terraform
# comment: false # Disable comment if false.
---

Yesterday I used the Infrastructure as Code, or IaC, tool [Terraform](https://developer.hashicorp.com/terraform/tutorials)
to build Azure cloud 
infrastructure for the [FlixTube](https://github.com/shantdashjian/flixtube) video streaming microservices-based 
system. Terraform is an open source project written in Go that provides a mechanism to use HCL, or Hashicorp 
Configuration Language, to automate the process of building cloud infrastructure using the HCL human-friendly 
configuration language, or code.

I specifically used it in combination with its Azure plugin, to set up the entire infrastructure on Azure cloud. I 
built a resource group, container registry, and 
the k8s cluster, and connected the cluster to the registry to pull the video streaming microservice Docker image.

The benefits of using IaC rather than doing all that manually via the Azure Portal (UI), or via the Azure CLI 
(terminal), is that using Terraform makes the process repeatable, reliable, and automated. This will then enable 
adding it as a step in the Continuous Delivery pipeline. It also enables you to track the changes you make to the 
infrastructure the same way to track the changes in your application code. It's because it's code you will place in 
GitHub.

### Three Terraform Commands
1. `terraform init`
2. `terraform apply`
3. `terraform destroy`
