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




Step 1 Create a Windows 10 VM and an Ubuntu server 20.04. Be sure to put them on the same Vnet.

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/65f8322c-0334-448d-b348-74673ee1c865)

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/fab04f5b-3d4e-47ad-93d1-ac72fe2fca23)

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/3014f392-353c-40d8-bf2f-b8826fd6005e)

Set the Ubuntu to Password instead of SSH key.

Step 2 Remote Access into the Windows 10 VM (VM1) using Remote Desktop Connection.

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/f7d4c549-4d9c-415d-adf9-bd617ce7b449)

Step 3 Download and Install Wireshark onto VM1.

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/cfa89b65-c259-4c49-91da-f536222f137a)

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/92237819-d0f6-45b0-9c83-e5fe872be516)

Step 4 Open Powershell and wireshark, then filter for ICMP traffic on wireshark. Ping the Private IP of the Ubuntu VM2 and observe the ICMP traffic

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/a6be752e-0e3a-4a60-ab1a-4c25ae2a1271)

Step 5 Disabling ICMP traffic on VM2 and seeing the ping fail.

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/f0b09f42-25e7-4187-acd6-fb72687796c8)

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/71ce4aaa-11ce-466e-bc0c-b959ee6e5acd)

Step 6 SSH into VM2 and create a txt. document.

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/ba5d605e-0126-40cc-b48c-ddebbfb99b34)

Step 7 Observe DHCP traffic with ipconfig /renew

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/57f95b66-ffad-4de1-853e-18b5b2254c37)

Step 8 DNS looking up IPs for websites

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/e9e125e9-babb-4928-8495-fbd0b375fd7e)

Step 9 RDP Traffic, since I'm remoting into VM1 this shows that traffic.

![image](https://github.com/KitchReeves/azure-network-protocols/assets/158783649/7ad6e276-6351-4730-9088-53ff4e0c7032)






