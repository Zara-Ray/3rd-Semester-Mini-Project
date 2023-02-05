### TERRAFORM AND ANSIBLE

* Using Terraform to create 3 EC2 instances and put them behind an Elastic Load Balancer

* After applying terraform plan, Terraform will: <br>
  ~ export the public IP addresses of the 3 instances to a file called host-inventory

* Setting up a domain with AWS Route53 within the terraform plan, and adding an A record for subdomain terraform-test that points to the ELB IP address

* Creating an Ansible script that:<br>
  ~ uses the host-inventory file Terraform created to install Apache <br>
  ~ sets timezone to Africa/Lagos <br>
  ~ displays a simple HTML page that displays content to clearly identify on all 3 EC2 instances.

