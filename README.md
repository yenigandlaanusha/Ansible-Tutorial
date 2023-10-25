# Ansible-Tutorial

What is Ansible?

Ansible is a powerful  open source automation tool that can help you manage and configure your server,applications and infrastructure effortlessly.

Why use Ansible?

Simplicity: Ansible uses plain English and YAML files for configuration , making it accessible to everyone.

Agentless:You don't need to install agents on traget servers.Ansible works over SSh or WinRM,which most systems support by default

Versatility:It can handle a wide range of tasks, from simple server configuration to complex application deployments

**Introduction to Ansible**

Ansible Components

Control Node : This is your Ansible machine,where you write your playbooks and manage everything from

Managed Nodes : These are the servers or devuces you want to automate: Ansible communicates with them using ssh (linux) and winRM (windows)

Playbooks : Think of them as receipes.Playbooks define the tasks you want to perform on your managed nodes

Modules : These are Ansibles's building blocks.Modules are used to execute tasks such as installing software or creating files.



**Setting up your Environment**

Install Ansible: sudo apt-get install Ansible

Add Inventory File : In Inventory file, we add the IP address of managed nodes

For Linux SSH key : Generate ssh-keygen and add your public key in target nodes

Test the connection : ansible -m ping -i inventory all
