---
layout: post
title: Serverless architectures
date: 2020-03-10T13:57:53.192Z
---

Brief notes on Serverless architectures

- Supports backend components like,
  - Compute (AWS Lambda functions)
  - Database (Firebase)
  - Storage
  - Stream processing
  - Message queueing
- Don't require provisioning, maintenance for the above components
- Fault tolerance and availability is handled internally
- Application is run in stateless compute containers that are event triggered
- This event can be triggered from various places, defined the provider, in case of AWS, it can be S3 updates,
time (scheduled tasks), messages received from message bus (Kinesis)
- To spin these containers up, the providers use 2 types of startup mechanism,
  - Warm start
    - Reusing of an instance from the previous event
  - Cold start
    - Creating a new container instance
    - The cold start latency is dependent on many variables like, the language used, the libraries used, how much code you have.
    - The cold start is also dependent on the frequency of which the event is triggered. 

