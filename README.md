<p align="center">
<img src="" alt=""/>
</p>

<h1>Setting Up and Configuring Cisco Router and Switch</h1>
This tutorial outlines the  installation of a Cisco 4351ISR router and a Cisco 3560-X Switch aswell as how to configure it for an organization.<br />



<h2>Environments and Technologies Used</h2>

- Routing
- DHCP
- DNS
- Firewalls
- APs
- 802.11
- VLANS
- Switching
- Cisco CLI


<h2>Operating System </h2>

- Windows 10</b> (22H2)
- Cisco CLI


<h2>Installation Steps</h2>

<p>
The first step is plugging both of the units into power and testing them before putting them on the rack, then connecting the internet from the modem into the back of the router, then connecting the WAN port from the router to the first port on the switch.
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/8a0ab042-63a5-4445-94d4-1385cb908a2e" height="80%" width="80%"/>
</p>
<br />

<p>
Next I used PuTTy to connect to the Routers console port, then later to the switches console port.
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/f85090b0-3bd7-44b7-85d1-a9f6d57199bb" height="80%" width="80%"/>
</p>
<br />


<p>
Now when in putty I typed enable and then configure terminal to get into the configureation mode
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/9f9306ce-a739-4907-9bb8-a91f67942d8e" height="80%" width="80%"/>
</p>
<br />

<p>
Then I defined the port 0/0/0 on the back of the router as the WAN to Modem connection
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/b77745c7-12d5-493d-8027-50cc2fcfd24a" height="80%" width="80%"/>
</p>
<br />

<p>
Next I defined the port 0/0/1 as the LAN to Switch connection and assigned it an IP address
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/b318ddfa-f847-4e0c-8af0-131beb9bb13a" height="80%" width="80%"/>
</p>
<br />

<p>
Next using these commands I enabled NAT and defined the modem and switch ports as outside and inside of the LAN respectively, This allows every device on the LAN to share a single public IP address
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/cfec56b2-41bd-422f-80c5-48086f584200" height="80%" width="80%"/>
</p>
<br />

<p>
Next I set up the DHCP server and the DNS server
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/2d2fa8a9-119e-4123-a5ac-5ba3d2650ba2" height="80%" width="80%"/>
</p>
<br />

<p>
I then saved this config to the routers memory
  </p>
<p>
  <img src="https://github.com/user-attachments/assets/9e652bf4-d772-40de-8de4-9be6394bf8af" height="80%" width="80%"/>
</p>
<br />

<p>

  </p>
<p>
  <img src="https://github.com/user-attachments/assets/a153a554-4ece-4760-926d-ff228660b7bb" height="80%" width="80%"/>
</p>
<br />

