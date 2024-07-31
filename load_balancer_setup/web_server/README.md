**Ansible Playbook: Configure and Manage HTTPD Web Server**

This Ansible playbook installs and configures an HTTPD web server. It ensures the HTTPD package is installed, deploys a custom web page, and makes sure the HTTPD service is running.

**Requirements**

Ansible 2.9 or later
A supported Linux-based system (e.g., CentOS, Ubuntu)

**Variables**

Variables are used in this playbook. You can override those variables in your playbook or in a separate variables file.

**Tasks**

*Install HTTPD Package*:
Uses the package module to ensure that the HTTPD package is installed. The package name is specified by the httpd_package variable.

*Copy Web Page Content*:
Uses the copy module to deploy a custom HTML file to the web server's document root. The content of the web page is specified by the web_page_content variable, and the destination path is specified by web_page_dest.

*Ensure HTTPD Service is Running*:
Uses the service module to start the HTTPD service and ensure it is running. The service name is specified by the httpd_service variable.

**Dependencies**

This playbook does not have any external dependencies.

**Contribution**

Contributions are welcome! If you have any improvements or fixes, please open an issue or submit a pull request.













