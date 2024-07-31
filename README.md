**Ansible Setup and Configuration Guide**

This guide provides instructions for setting up an Ansible inventory, creating an EC2 instance, and configuring connections between a load balancer role and a web server role. Follow the steps below to complete each task.

**1. Create EC2 Instance**

This section describes how to create an EC2 instance using Ansible.

*Instructions*
- Set Up AWS Credentials: Replace "Enter access key to login to aws" and "Enter secret key to login to aws" with your actual AWS credentials. It is recommended to use environment variables or AWS Secrets Manager for securely managing these credentials.
- Run the Playbook: Execute the playbook with the following command: 
  "ansible-playbook aws_ec2_instance_setup.yml"
- Verify Instance Creation: Check the output for the instance ID and verify the EC2 instance creation in your AWS Management Console.

**2. Ansible Inventory Setup**

Ansible inventory defines the hosts and groups of hosts that Ansible manages. You need to create an inventory file to specify the servers that Ansible will manage.

**3. Setup Connection Between Load Balancer Role and Web Server Role**

To connect a load balancer role and a web server role, you need to configure them so that the load balancer can distribute traffic to the web servers.

**Dependencies**

This playbook does not have any dependencies outside of Ansible.

**Contribution**

Contributions to this setup guide or the Ansible roles are welcome. Please open issues or submit pull requests if you have suggestions or improvements.
