#-------------------------------------------------------------------------------------------------------------------------------------------------------------
# INTRODUCTION
#-------------------------------------------------------------------------------------------------------------------------------------------------------------

# VMware

- Provides cloud computing and platform virtualisation software and services.
- Has **type1** hypervisors that run directly on server hardware without requiring an additional underlaying operating system.<br/>


## What is virtualisation
To create a virtual version of a device or resource. i.e (server, storage device, network, OS)<br/>

- devices, applications and human users are able to interact with virtual resource as if it were a real single resource
- disk partition is an example of virtualisation


## What is a hypervisor 
<br/>
> A virtual machine monitor(VMM). computer software, firmware or hardware that creates and runs virtual machines.
<br/>

### Types of Hyperviser
<br/>

**Type 1:**<br/>
Bare metal Hypervisor<br/>

- runs directly on the hardware (firmware)

**Type 2:**<br/>
Host OS Hypervisor<br/>

- An operating system that has a hypervisor (software)







# What is VMware: vSphere ESXi and vCenter
<br/>



## vSphere ESXi

- ESXi is type 1 Hypervisor firmware
	- Allows for basic creation and management of virtual machines and networking
	- 
- vSphere manageement interface provides access on a per server basis and is accessed by browsing to the IP of ESXi host



## vCenter

> Central management interface to manage all ESXi hosts and VMs<br/>
- use it configure the ESCXi Hosts



#-------------------------------------------------------------------------------------------------------------------------------------------------------------
# CONFIGURATION WITH TERRAFORM
#-------------------------------------------------------------------------------------------------------------------------------------------------------------


# Terraform and VMware

#-------------------------------------------------------------------------------------------------------------------------------------------------------------
# CONFIGURATION WITH ANSIBLE 
#-------------------------------------------------------------------------------------------------------------------------------------------------------------

# Ansible and VMware

> To confifure Ansible for VMware:<br/>
- Install pyVmomi
- Install community.vmware
(Ansible Docs)
- create inventory & playbook

(Ansible Piolt,2022)

To use ansible to configure VMware I need to configure ansible to be able to use VMware modules.<br/>
Using:<br/>
ansible-galaxy install collection community.vmware<br/>

- I download the VMware collection and added it into my working directory under the collections folder.
- added an ansible.cfg file within working directory so that ansible would search for the newly added collection within the working directory
(madapparambath, 39:05)

- wrote the script that should aid in creating a vm off of the vmware firmware. I dont have log-in credentials and I dont have the ip address of the machine to test it out.









# References
- edureaka, 2018, [youtube], VMware Tutorial for Beginners | VMware Workstation | VMware virtualisation | Edureka [online] accessed 16/11/2022. link (https://www.youtube.com/watch?v=7m3f-P-WWbg)<br/>
- Rob Willis, 8 jul 2017, [youtube], What is VMware vSphere ESXi and vCenter, [online] accessed 16/11/22, link (https://www.youtube.com/watch?v=-Hltydu9PXk)<br/>
- Davanzo, A 25 jul 2018, [Blog], Using Ingrastructure as Code to Automate VMware Deployments, [Online] visited 17/11/2022, link: (https://www.hashicorp.com/blog/using-infrastructure-as-code-to-automate-vmware-deployments)
- Future on Cloud, 3 December 2021, [YouTube] Create VM using Ansible and Playbook [online] visited 17/11/22, link:(https://www.youtube.com/watch?v=6zGci2yRkqI)
- Ansible Pilot, n/a, [website] Welcome to Ansible Piolt [online] visited 17/11/22 link: (https://www.ansiblepilot.com)
- Madapparambath.G, 22 December 2020, techbeatly[blog] Getting Started with Ansible Collections, [online] visited 17/11/22 link:(https://www.techbeatly.com/getting-started-with-ansible-collections/#:~:text=So%20basically%2C%20Ansible%20Collections%20are,plugins%2C%20filters%20and%20Ansible%20Roles.)
- techbeatly.com, (n/a), [website] Ansible Automation, [online] visited 17/11/22, link:(https://www.techbeatly.com/ansible/)
- Ansible Pilot, 16 May 2022, [YouTube], Configure Ansible for VMware - ansible collection community.vmware [online] accessed 17/11/22, link (https://www.youtube.com/watch?v=suDlOTt6n_Y&list=PLButRaJV74S5YNOEZhdhW38slbjdQWEe7)
- Ansible Docs, (n/a),[Website] community.vmware.vmware_guest module - Mangages virtual machines in vCenter [online] accessed 18/11/22, link, (https://docs.ansible.com/ansible/latest/collections/community/vmware/vmware_guest_module.html#ansible-collections-community-vmware-vmware-guest-module)
- NLB Solutions, 7th Feburary 2018,[Youtube] Introduction to VMware vSphere 6.5 [online] accessed 18/11/22. link (https://www.youtube.com/watch?v=qyZnAf7U2FQ)

