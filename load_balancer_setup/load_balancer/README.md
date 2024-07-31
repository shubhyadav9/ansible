**Ansible Playbook: Configure and Manage HAProxy**
This Ansible playbook configures and manages HAProxy. It installs HAProxy, sets up its configuration using a Jinja2 template, and ensures the HAProxy service is running. The playbook is designed to be run on all hosts in the inventory and requires elevated privileges.

**Requirements**
Ansible 2.9 or later
A Linux-based system where HAProxy can be installed (e.g., CentOS, Ubuntu)
