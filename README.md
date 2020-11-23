# cybersecurity
Projects from cybersecurity certificate class.
## Automated ELK Stack Deployment

The files in this repository were used to configure the network depicted below.

![Final Diagram Map](Images/Final Diagram Map.png)

These files have been tested and used to generate a live ELK deployment on Azure. They can be used to either recreate the entire deployment pictured above. Alternatively, select portions of the install-elk.yml file may be used to install only certain pieces of it, such as Filebeat.

  - file-playbook2.yml.txt_

This document contains the following details:
- Description of the Topologu
- Access Policies
- ELK Configuration
  - Beats in Use
  - Machines Being Monitored
- How to Use the Ansible Build


### Description of the Topology

The main purpose of this network is to expose a load-balanced and monitored instance of DVWA, the D*mn Vulnerable Web Application.

Load balancing ensures that the application will be highly available, in addition to restricting access to the network.
- What aspect of security do load balancers protect? Availability
What is the advantage of a jump box? Decreases attack surface area

Integrating an ELK server allows users to easily monitor the vulnerable VMs for changes to the files and system resources.
-  What does Filebeat watch for? Changes to file system
- _What does Metricbeat record? Changes to services on the machines

The configuration details of each machine may be found below.
_Note: Use the [Markdown Table Generator](http://www.tablesgenerator.com/markdown_tables) to add/remove values from the table_.

| Name     | Function | IP Address | Operating System |
|----------|----------|------------|------------------|
| Jump Box | Gateway  | 10.0.0.4   | Linux            |
| Web 1    | Web      | 10.0.0.8   | Linux            |
| Web2     | Web      | 10.0.0.9   | Linux            |
| Web3     | Web      | 10.0.0.5   |                  |

### Access Policies

The machines on the internal network are not exposed to the public Internet. 

Only the jump box machine can accept connections from the Internet. Access to this machine is only allowed from the following IP addresses:
- 69.218.225.78
