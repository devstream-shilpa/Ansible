Summary
This work automates the deployment of web servers on two virtual machines (VMs) using Ansible. The process involved several key steps:

Virtual Machine Setup: I created and configured two Ubuntu Server VMs (VM1 and VM2) in VirtualBox, ensuring they had network connectivity to my local machine.

Ansible Installation: I installed and configured Ansible on my Mac, which served as the control machine for the deployment.

Project Creation: I created a standard Ansible project with an inventory file (inventory.ini) to manage the VMs and two playbooks (deploy.yml, un-deploy.yml) to handle deployment and removal of resources.

Deployment: I ran the deploy.yml playbook to install and configure the Nginx web server on each VM, including:

Installing the Nginx package.

Adding a firewall rule to allow web traffic on port 8080.

Creating a custom "Hello World" web page on each server.

Troubleshooting: The project involved troubleshooting common issues, including SSH connection timeouts and firewall-related service failures.

Final Verification: After successfully running the playbook, I verified that the web servers were running by accessing their web pages in a browser.
