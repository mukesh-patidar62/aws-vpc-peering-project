# Architecture notes

- VPC A: `10.10.0.0/16`; public subnet `10.10.1.0/24`; private subnet `10.10.2.0/24`.
- VPC B: `10.20.0.0/16`; private subnet `10.20.1.0/24`.
- Bastion is in the public subnet in VPC A; app instances are private-only.
- VPC peering is point-to-point and non-transitive.
- Routes are required in both directions; peering alone does not add routes.
- Security groups and network ACLs can still block traffic.
