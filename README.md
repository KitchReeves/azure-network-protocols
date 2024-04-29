<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04




Step 1 Create a Windows 10 VM and an Ubuntu server 20.04. Be sure to put them on the same Vnet

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/65f8322c-0334-448d-b348-74673ee1c865)

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/fab04f5b-3d4e-47ad-93d1-ac72fe2fca23)

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/3014f392-353c-40d8-bf2f-b8826fd6005e)

Set the Ubuntu to Password instead of SSH key.

Step 2 Remote Access into the Windows 10 VM (VM1) using Remote Desktop Connection.

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/f7d4c549-4d9c-415d-adf9-bd617ce7b449)

 




