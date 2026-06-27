# Lesson 8 – VPC and Subnets

## Learning Objectives

- Understand what a VPC is.
- Understand Subnets.
- Differentiate Public and Private Subnets.

---

## What is a VPC?

VPC stands for **Virtual Private Cloud**.

A VPC is your own private network inside AWS.

Think of it as your own fenced estate inside Amazon's cloud.

Benefits:

- Network isolation
- Security
- Full control over IP ranges
- Custom routing
- Resource organization

---

## What is a Subnet?

A subnet is a smaller network inside a VPC.

Subnets help separate resources based on security and function.

---

## Public Subnet

A subnet that can communicate directly with the internet through an Internet Gateway.

Typical resources:

- Web Servers
- Load Balancers
- Bastion Hosts

---

## Private Subnet

A subnet that does not allow direct inbound access from the internet.

Typical resources:

- Databases
- Backend Servers
- Redis
- Internal APIs

---

## Key Takeaways

- A VPC is your private AWS network.
- A subnet is a smaller network inside a VPC.
- Public subnets allow internet access.
- Private subnets protect sensitive resources.