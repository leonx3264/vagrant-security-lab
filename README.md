# vagrant-security-lab
A demo security lab using vagrant boxes and virtualbox.

Software Requirements:
  - Vagrant
  - VirtualBox
  - Oracle VM VirtualBox Extension Pack

Hardware Requirements:
  - 4 Core 8 Threads CPU
  - 16GB+ Memory (9GB used by VMs on boot)
  - 70GB Storage (33GB used by VMs on boot)

Creates 4 Virtual Machines:
  - Kali-Box (Rolling Kali instance, GUI enabled by default)
  - OWASP-Box (CentOS instance, JuiceBox (with ModSecurity), WebGoat, WebWolf installed)
  - DVWA-Box (Ubuntu instance, DVWA installed)
  - MSF3-Box (Win Server 2008, Metasploitable3 installed)

Credentials for all VMs are vagrant:vagrant

Addresses:
  - Kali-Box:       172.16.20.121
  - OWASP-Box:      172.16.20.10
  - DVWA-Box:       172.16.20.20
  - MSF3-Box:       172.16.20.30
