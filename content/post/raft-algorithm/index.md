---
title: "Raft Algorithm" # Title of the blog post.
date: 2023-08-06T13:40:41+04:00 # Date of post creation.
tags:
  - raft
  - consensus algorithm
# comment: false # Disable comment if false.
---

Yesterday I looked at the [Raft consensus algorithm](https://raft.github.io/) for distributed systems. It's an 
algorithm to enable a group of servers/nodes to reach an agreement on a value. It's 
meant to 
replace a previous consensus algorithm called Paxos which was perceived to be complicated and difficult to 
understand. Raft on the other hand is easier to understand. It consists of two phases:
1. Leader Election
2. Log Replication

For a visual explanation of Raft, see [this](http://thesecretlivesofdata.com/raft/).

**Raft** stands for Replicable, Reliable, Redundant and Fault-Tolerant.
