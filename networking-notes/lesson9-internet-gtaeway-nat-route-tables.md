# Lesson 9 – Internet Gateway, NAT Gateway & Route Tables

## Internet Gateway (IGW)

- Connects a VPC to the Internet.
- Required for public internet access.
- Used by Public Subnets.

---

## Route Table

A Route Table tells AWS where to send network traffic.

Example:

| Destination | Target |
|------------|---------|
| 10.0.0.0/16 | Local |
| 0.0.0.0/0 | Internet Gateway |

---

## NAT Gateway

Allows resources in a Private Subnet to access the Internet without allowing inbound Internet connections.

Examples:

- Download software updates
- Install packages
- Access GitHub

---

## Key Differences

Internet Gateway:
- Public access
- Internet can initiate connections

NAT Gateway:
- Private outbound access
- Internet cannot initiate connections

---

## Key Takeaways

- Public Subnets use an Internet Gateway.
- Private Subnets use a NAT Gateway for outbound Internet access.
- Route Tables determine where traffic goes.