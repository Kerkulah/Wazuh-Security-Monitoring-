<h1> Wazuh Security Monitoring
</h1>



<h2>Lab Environment Overview</h2>
This lab demonstrates how attackers perform password based SSH attacks using tools like Hydra and how security teams can detect and respond to these attacks using a Security Information and Event Management (SIEM) system. The environment consists of three core components working together to simulate a complete attack and defend scenario.
<br />
<br />

<br /> Active Agents: <br />
<img src="https://imgur.com/U4Ry2nZ.jpg"  height="80%" width="80%">
<br /> Agent 001 (Kali) - Kali GNU/Linux 2025.1 - Attacker machine <br />
<br />Agent 004 (Ubuntu-Desktop) - Ubuntu 24.04.3 LTS - Target/Victim machine<br />
<br />Cluster: node01<br />
<br />Version: v4.14.2<br />
<br />
<br />

<br />
<h2> Tech Stack</h2>

Proxmox VE : https://www.virtualbox.org/wiki/Downloads](https://www.proxmox.com/en/downloads
<br />
<br />
Kali Linux :                             https://www.kali.org/get-kali/#kali-installer-images
<br />
<br />
Ubuntu Desktop :                                https://ubuntu.com/tutorials/how-to-run-ubuntu-desktop-on-a-virtual-machine-using-virtualbox#1-overview

Wazuh :                                https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html
<br />
<h2> Brute Force Detection</h2>
<br />
Using Hydra Simulate SSH brute force attack and detect it with Wazuh.
<br />
<br />
<br /> -Install HYDRA on my Kali system <br />
<br />- Created  a small password list<br />
<br />
<br />
<img src="https://imgur.com/UeAnw3B.jpg"  height="80%" width="80%">
<br />
<br />
<br />On Wazuh Dashboard, filter for Multiple authentication failures and check for Possible SSH brute force attack. <br />
<br />
<br />
 - Multiple authentication failures (rule.id:5710)
<img src="https://imgur.com/AItOkyC.jpg"  height="80%" width="80%">

<img src="https://imgur.com/JjpuPrc.jpg"  height="80%" width="80%">
<br />- Possible SSH brute force attack (rule.id:5712) <br />
<img src="https://imgur.com/WX8VHs6.jpg"  height="80%" width="80%">
<img src="https://imgur.com/iPoux4P.jpg"  height="80%" width="80%">
<br />
<br />
<br />

<p align="center">
<br/>
<h1> File Integrity Monitoring </h1>
 
<br />
- On Ubuntu, monitor critical files and detect unauthorized changes
<br />
<img src="https://imgur.com/r1X23Tn.jpg"  height="80%" width="80%">
<img src="https://imgur.com/nNWqgcZ.jpg"  height="80%" width="80%">

<br />
<br />
 <h1>Ubuntu Server, Docker, Portainer installed, verified, and accessible
 </h1>
<br />
 <br/>
<img src="https://imgur.com/sVUYYP0.jpg"  height="80%" width="80%">
<br />
<br />
<h1> Metasploitable2 VM created, and MACVLAN networking configured bWAPP, DVWA, and WebGoat deployed. All vulnerable machines are reachable for future security tool integration.
</h1>
<br/>
<br />
<br />
<img src="https://imgur.com/sUjhHat.jpg"  height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/aG3GE3h.jpgh"  height="80%" width="80%">
<br />

<br />
<br />
<br />
<h1> Wazuh server, Nessus Essential Integration of both tools into VLAN 10 (security tools segment). Firewall rule adjustments for scanning and agent communication. Initial vulnerability scans against Metasploitable2, DVWA, bWAPP, and WebGoat. </h1>
<br />
<br />
<img src="https://imgur.com/Prw149V.jpg"  height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/M2dsQUb.jpg"  height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/PgGwCDc.jpg"  height="80%" width="80%">
<br />
<br />
<br />
<br />

<h1> Adding Windows enterprise environment to the lab. Build a Windows Server 2022 Domain Controller and a Windows 10 workstation, then configure Active Directory, DNS, DHCP, and Group Policy.  </h1>
<br />
<br />
<img src="https://imgur.com/OVDGZbC.jpg"  height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/XW2c2Cb.jpg"  height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/2OxqR10.jpg"  height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/ODmGUuu.jpg"  height="80%" width="80%">
<br />
<br />
<h1>Build a site‑to‑site VPN between pfSense and an Azure VNet. This unlocks the ability to run cloud resources. Creating Azure resources (Resource Group, VNet, subnets, VPN Gateway, Local Network Gateway)
 Handling home‑network constraints (dynamic public IP, port forwarding, static WAN assignment)
 </h1>
<br />
<br />
<img src="https://imgur.com/ryUcznH.jpg"  height="80%" width="80%">
<br />
<br />
<img src="https://imgur.com/4B5dvAV.jpg"  height="80%" width="80%">
<br />
<br />
<br />
<img src="https://imgur.com/1AANkAr.jpg"  height="80%" width="80%">
<br />
<br />


