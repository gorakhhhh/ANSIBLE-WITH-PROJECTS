# 🚀 Ansible Automation – Complete Practical Guide

Welcome to my Ansible automation repository!

This repository contains hands-on practicals, configuration examples, playbooks, and real-world automation projects using Ansible. It focuses on managing multiple Linux servers from a single control node, reducing manual administration, and automating repetitive system administration tasks.

Ansible is an open-source automation tool used for configuration management, application deployment, and infrastructure automation. It uses inventory files, YAML-based playbooks, and modules to execute tasks on managed hosts, typically over SSH. <Cite refs={["turn422529view0","turn422529view1"]}/>

## 📚 Topics Covered

### 1. Introduction to Ansible
- What is Ansible?
- Ansible architecture and components.
- Control node and managed nodes.
- Agentless automation and SSH connectivity.
- Configuration management and orchestration.
- Advantages and use cases of Ansible.

### 2. Ansible Installation
- Install Ansible on a Linux control node.
- Verify the Ansible installation.
- Configure SSH connectivity.
- Set up passwordless SSH authentication.
- Prepare managed Linux servers.
- Test connectivity using Ansible ad hoc commands.

### 3. Ansible Configuration File
- Understand `ansible.cfg`.
- Configure the default inventory.
- Set the remote user and SSH options.
- Configure privilege escalation.
- Understand configuration precedence.
- Customize Ansible execution settings.

### 4. Inventory and Host Management
- Create static inventory files.
- Add multiple Linux servers.
- Group servers by application or environment.
- Configure host-specific variables.
- Configure group variables.
- Test connectivity to all hosts.
- Manage different server groups using host patterns.
- Explore dynamic inventory concepts.

### 5. Ansible Ad Hoc Commands
- Execute commands on remote hosts.
- Check connectivity using the ping module.
- Collect system information.
- Manage packages and services.
- Execute commands across multiple servers.
- Use privilege escalation with `-b`.

### 6. Ansible Playbooks
- Understand YAML syntax.
- Create and execute playbooks.
- Define plays, tasks, and handlers.
- Use built-in Ansible modules.
- Validate playbook syntax.
- Execute playbooks against selected hosts.
- Use check mode before applying changes.
- Understand idempotency and repeatable automation.

### 7. Variables and Facts
- Define variables in playbooks.
- Use inventory and group variables.
- Store variables in separate files.
- Pass variables through the command line.
- Collect facts from managed machines.
- Identify operating systems, IP addresses, and memory information.
- Use facts in conditional tasks.
- Understand variable precedence.

### 8. Loops and Conditions
- Repeat tasks using `loop`.
- Create multiple users using a single task.
- Install multiple packages.
- Use `when` conditions.
- Run tasks based on operating system facts.
- Register command results.
- Handle task outcomes and failures.

### 9. User and Group Management
- Create users on multiple Linux servers.
- Create groups and assign users.
- Configure home directories and login shells.
- Manage user account settings.
- Remove users when required.
- Configure authorized SSH keys.
- Automate user administration across host groups.

### 10. Package Management
- Install packages on multiple servers.
- Remove unwanted packages.
- Update selected packages.
- Manage packages on RHEL-based systems.
- Manage packages on Ubuntu and Debian.
- Use the appropriate package modules for each operating system.

### 11. Service Management
- Start services across multiple machines.
- Stop and restart services.
- Enable services at boot.
- Disable services when required.
- Check service status.
- Install a package and start its service.
- Use handlers to restart services after configuration changes.

### 12. Firewall Management
- Manage firewall services on Linux servers.
- Install and configure firewalld where supported.
- Start and enable the firewall service.
- Open and remove firewall ports.
- Configure permanent firewall rules.
- Verify active firewall settings.
- Manage firewall rules using suitable Ansible modules and collections.

### 13. Roles and Collections
- Understand reusable Ansible roles.
- Create roles using `ansible-galaxy`.
- Organize tasks, handlers, variables, templates, and files.
- Reuse roles across different projects.
- Understand Ansible collections.
- Install and use community collections.
- Use fully qualified collection names in playbooks.

### 14. Ansible Project Structure
- Organize inventories and playbooks.
- Create separate development and production inventories.
- Maintain reusable variables and roles.
- Store projects in GitHub.
- Use Ansible Vault to protect sensitive information.
- Build maintainable automation projects.

## 🖥️ Real-World Projects

### Project 1: Manage Multiple Linux Servers from One Control Node

Configure one Ansible control node to manage multiple remote Linux machines using SSH and an inventory file.

Automate tasks such as:
- Check connectivity to all managed hosts.
- Collect hostname and operating system information.
- Create users and groups.
- Install and remove packages.
- Start, stop, and restart services.
- Configure firewall services and ports.
- Execute administrative tasks across selected host groups.

### Project 2: Automated User Creation on All Hosts

Create a playbook that creates a specified user on multiple Linux servers, configures the required groups, and creates the home directory.

The playbook can manage the desired user state consistently across all targeted machines.

### Project 3: Install and Manage Services Across Multiple Hosts

Create playbooks to install a service such as Apache HTTP Server, start it, enable it at boot, and verify its status across multiple servers.

Additional playbooks can stop, restart, disable, or remove the service when required.

### Project 4: Firewall and Port Configuration

Automate firewall administration across managed servers by configuring the firewall service and allowing required ports, such as HTTP port 80 or HTTPS port 443.

Verify the resulting configuration and avoid changing remote-access rules in a way that could lock you out.

### Project 5: Automated Server Configuration

Build a reusable role that configures Linux servers with required packages, users, services, and firewall rules. Use inventory groups and variables to apply different configurations to web servers and application servers.

## 🎯 Learning Objectives

After completing these practicals, learners should be able to:

- Install and configure Ansible.
- Manage several Linux servers from a central control node.
- Configure inventory files and SSH connectivity.
- Write and execute YAML playbooks.
- Use variables, facts, loops, and conditions.
- Automate user and group administration.
- Install, remove, start, and stop services.
- Configure firewall services and ports.
- Build reusable roles and use collections.
- Organize projects for repeatable infrastructure management.
- Apply automation techniques in cloud and DevOps environments.

## 🛠️ Recommended Lab Environment

- One Linux control node with Ansible installed.
- Two or more Linux managed nodes.
- SSH connectivity between the control node and managed nodes.
- A suitable remote account with required sudo privileges.
- VMware, VirtualBox, or cloud-based virtual machines.
- Git and GitHub for version control.

## ☁️ Ansible for Cloud and DevOps

Ansible can help automate server configuration and application deployment on Linux machines hosted in AWS, Microsoft Azure, and other environments.

It can also complement Terraform, Docker, Kubernetes, and CI/CD pipelines by automating post-provisioning configuration and routine administration.

## 🔐 Best Practices

- Use SSH keys or other approved secure authentication methods.
- Apply least-privilege access.
- Store sensitive values using Ansible Vault.
- Validate playbooks before execution.
- Use check mode when supported by the tasks.
- Test destructive changes in a lab first.
- Use idempotent modules wherever possible.
- Keep playbooks and inventory examples under version control without committing secrets.

## 👨‍💻 About the Author

**Gorakhnath Malusare**

Cloud Computing | AWS | Microsoft Azure | Linux | Networking | Ansible | DevOps

I am passionate about cloud computing, Linux administration, automation, and DevOps. I build practical labs and documentation to strengthen my technical skills and share hands-on learning resources.

🔗 GitHub Profile: https://github.com/gorakhhhh

## ⭐ Support

If you find this repository helpful, consider giving it a star ⭐ and sharing it with other learners.

**Automate tasks. Manage servers. Build reliable infrastructure.** 🚀
