---
layout: post
title: Subnets in AWS
date: 2020-03-01T13:57:53.192Z
---
A subnet is a range of IP addresses in your VPC

- If a subnet is connected to the internet gateway then it is a `public subnet`. It must have IPv4/IPv6 or Elastic IP address.
- If a subnet is not connected to the internet gateway then it is a `private subnet`.
- If a subnet is connected to a virtual private gateway, then it is a `vpn-only subnet`.
- Default subnets
    - Defined in default VPC in each availability zone
- Non-Default subnets
    - Defined in non-default VPC and additionally created subnets in default VPC
    - Instances in these subnets have private IPs. You can attach public IPs yourself. 
    - To enable internet access
      - attach public IP (or Elastic IP)
      - attach to internet gateway 
