
This Terraform project creates a Virtual Private Cloud (VPC) in AWS and sets up four subnets, two public and two private. 
The public subnets are used for the bastion host and the NAT gateway, while the private subnets are used for the EC2 instance.
The project deploys an EC2 instance in one of the private subnets, which is not accessible from the outside world. 
To access the instance, the project sets up a bastion host in one of the public subnets. The bastion host acts as a gateway to the private subnet, allowing secure access to the EC2 instance.
The project also sets up a NAT gateway in one of the public subnets, which allows the EC2 instance in the private subnet to access the internet. 
The NAT gateway provides a secure way for the private subnet to access the internet without exposing it to the public.
