# NAT gateways

A NAT gateway is a Network Address Translation(NAT) service.
You can use a NAT gateway so that instances in a private subnet can connect to services outside your VPC but external services can't initiate a connection with those instances.

The NAT gateway replaces the source IP
address of the instances with the IP address of the NAT gateway. For a public NAT gateway, this is the elastic IP address of the NAT gateway. For a private NAT gateway, this is the private IPv4 address of the NAT gateway. When sending response traffic to the instances, the NAT device translates the addresses back to the original source IP address.

NOTE:
NAT Gateway usually deployed at public subnet so that connection between outside of VPC and private subnet can be connected.
