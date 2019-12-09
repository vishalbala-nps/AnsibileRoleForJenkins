# AnsibileRoleForJenkins
An Ansible role for installing Jenkins on Fedora
## Overview
This is an Ansible role for automating the installation of Jenkins on Red-Hat based distributions (like Fedora, Red Hat, CentOS etc.)
## Requirements
 - You need to have a user on the remote server configured with passwordless sudo. 
 - The remote server should also have ssh configured based on Ansible's requirements
## How to Use
 - Begin by first cloning the repository with the command:  `git clone https://github.com/vishalbala-nps/AnsibileRoleForJenkins`
- Change the IP Address of the remote server in the inventory file and change the remote server username in the test.yml file
- Run the role by typing the command `ansible-playbook -i inventory test.yml`
- Once the Installation process has been completed, it will display the initial password to access Jenkins. You can access Jenkins and complete initial setup by going to: [REMOTE_SERVER_IP]:8080 in your browser
## Reference
- https://wiki.jenkins.io/display/JENKINS/Installing+Jenkins+on+Red+Hat+distributions I used the commands in this site and automated it with Ansible
## What is Jenkins?
Jenkins is an open-source, Java based automation software. It is used by many companies around the world. It can be used to automate tasks related to building, testing, and delivering or deploying software.
