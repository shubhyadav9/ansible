**Ansible Playbook: Configure and Manage HAProxy**

This Ansible playbook configures and manages HAProxy. It installs HAProxy, sets up its configuration using a Jinja2 template, and ensures the HAProxy service is running. The playbook is designed to be run on all hosts in the inventory and requires elevated privileges.

**Requirements**

Ansible 2.9 or later
A Linux-based system where HAProxy can be installed (e.g., CentOS, Ubuntu)

**Variables**

Variables are used in this playbook. You can override these variables in your playbook or in a separate variables file.

**Tasks**

*Install HAProxy Package:*
Uses the package module to ensure that the HAProxy package is installed.

*Configure HAProxy Configuration File:*
Uses the template module to apply the HAProxy configuration from the Jinja2 template (haproxy.cfg.j2) to the specified destination path (/etc/haproxy/haproxy.cfg). This task triggers a handler to restart HAProxy if the configuration changes.

*Ensure HAProxy Service is Running:*
Uses the service module to start the HAProxy service and ensure it is running.

**Handlers**

*Restart HAProxy:*
A handler that restarts the HAProxy service if the configuration file is updated.

**Templates**

*haproxy.cfg.j2:* The Jinja2 template file used to generate the HAProxy configuration. This file should be placed in the templates/ directory.

**Dependencies**

This playbook does not have any dependencies outside of Ansible.

**Contribution**
Contributions to this playbook are welcome. Please feel free to open issues or submit pull requests if you have improvements or fixes.













