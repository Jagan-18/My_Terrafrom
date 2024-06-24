Overview of steps
Create a directory for your Terraform project and create a Terraform configuration file (usually named main.tf) in that directory. In this file, you define the AWS provider and resources you want to create. Here's a basic example:

   provider "aws" {
     region = "us-east-1"  # Set your desired AWS region
   }

   resource "aws_instance" "example" {
     ami           = "ami-0c55b159cbfafe1f0"  # Specify an appropriate AMI ID
     instance_type = "t2.micro"
