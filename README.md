# myterra
##my terrform
provider "aws" {
  region = "ap-south-1"
}

module "ec2-instance" {
  source = "github.com/Mohit7506/myterra"
  ami_id = "your ami-id"
  instance_type = "your instance_type"
  vpc_id = "your vpc_id"
  port = "port number"
  cidr_block = "0.0.0.0/0"
}
