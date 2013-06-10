# -*- mode: ruby -*-
# vi: set ft=ruby :

# From http://cloud-images.ubuntu.com/locator/ec2/
#
# name: precise
# version: 12.04 LTS
# arch: amd64
# instance type: ebs

Vagrant.configure("2") do |config|
  config.vm.provider :aws do |aws, override|
    aws.instance_type = "t1.micro"

    aws.region_config "ap-northeast-1", :ami => "ami-bb5ad2ba"
    aws.region_config "ap-southeast-1", :ami => "ami-bf8bc5ed"
    aws.region_config "ap-southeast-2", :ami => "ami-e9e675d3"
    aws.region_config "eu-west-1",      :ami => "ami-f1998985"
    aws.region_config "sa-east-1",      :ami => "ami-80d97c9d"
    aws.region_config "us-east-1",      :ami => "ami-e7582d8e"
    aws.region_config "us-west-1",      :ami => "ami-11e6c854"
    aws.region_config "us-west-2",      :ami => "ami-1d6ffe2d"

    override.ssh.username = "ubuntu"
  end
end
