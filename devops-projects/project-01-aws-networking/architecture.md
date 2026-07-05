# Architecture Design

## Overview

This document explains the AWS network architecture for the TayoTech production e-commerce application.

The architecture is designed to be secure, scalable, and highly available.

---

## Network Layout

The network contains:

- One VPC
- Public subnets
- Private subnets
- Internet Gateway
- NAT Gateway
- Route Tables
- Security Groups
- Application Load Balancer
- Web Servers
- Application Servers
- Database

---

## VPC Design

The architecture uses one VPC with the CIDR block:

```text
10.0.0.0/16