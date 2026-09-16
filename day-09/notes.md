# Day 9 - AWS EC2 Fundamentals

## What is Amazon EC2?

EC2 stands for Elastic Compute Cloud.

Amazon EC2 is an AWS service that provides virtual servers in the cloud.

Instead of purchasing and maintaining a physical server, we can create a virtual server using EC2.

## Why is EC2 used?

EC2 can be used to:

- Host websites
- Run applications
- Run backend services
- Process workloads
- Create development and testing environments

## EC2 Instance

An EC2 instance is a virtual server running in AWS.

When we launch an EC2 instance, we select different configurations such as:

- Operating system
- CPU
- Memory
- Storage
- Network settings

## AMI

AMI stands for Amazon Machine Image.

An AMI is a template used to create an EC2 instance.

It contains information such as:

- Operating system
- Application server
- Applications
- Required configuration

Example:

Amazon Linux AMI can be used to launch a Linux-based EC2 instance.

## Instance Type

An instance type determines the hardware configuration of an EC2 instance.

It defines resources such as:

- CPU
- Memory
- Network performance

Different instance types are designed for different workloads.

## Key Pair

A key pair is used to securely connect to an EC2 instance.

It consists of:

- Public key
- Private key

The private key must be kept secure.

## Security Group

A Security Group acts as a virtual firewall for an EC2 instance.

It controls inbound and outbound traffic.

Example:

We can allow HTTP traffic on port 80 so users can access a web server.

## Elastic IP

An Elastic IP is a static public IPv4 address that can be associated with an EC2 instance.

It can be useful when an application needs a consistent public IP address.

## EC2 Pricing

AWS provides different pricing options for EC2.

Common options include:

- On-Demand Instances
- Reserved Instances
- Spot Instances

## Scalability

EC2 allows us to increase or decrease computing resources according to workload requirements.

This helps organizations handle changing workloads.

## Important Terms

EC2 = Virtual server

AMI = Template used to launch an EC2 instance

Instance Type = CPU and memory configuration

Key Pair = Secure connection credentials

Security Group = Virtual firewall

Elastic IP = Static public IPv4 address
