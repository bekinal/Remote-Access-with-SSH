<h1>Remote Access with SSH</h1>

<h2>Description</h2>
Project consists of enabling SSH connections with RSA encryption. A switch is then set up with layer 3 connectivity and the SSH is tested by opening a session from a local PC.
<br />


<h2>Utilities Used</h2>

- <b>VirtualBox</b> 
- <b>Cisco Packet Tracer</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Configure SSH:</h2>
A console cable is used to make the connection between the switch and the admin PC. The switch is then connected through the terminal on the admin PC. The switch is given a device name and an Admin account. The enable password is set. All passwords are encypted on the device. A security message is set, and CyberPro.local is configured as the device domain: <br/>
<img src="https://imagizer.imageshack.com/img923/2162/O57IqA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Layer 3 connectivity is enabled on the switch giving it an IP address of 10.0.0.150 and subnet of 255.255.255.0. The interface is turned on by the "no shutdown" command. The default gateway is set as 10.0.0.1: <br/>
<img src="https://imagizer.imageshack.com/img924/1531/mb2Aqf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Remote access is permitted to the device. Line VTY is configured for local password checking. The line is set to display the banner creared when accessing the switch remotely. Only SSH connection requests are allowed to the switch: <br/>
<img src="https://imagizer.imageshack.com/img924/6835/PkmLub.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
RSA keys for the SSH process are created with a key length of 1,024 bits. The SSH version is configured to version 2: <br/>
<img src="https://imagizer.imageshack.com/img923/9397/Yt4diJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<h2>Verify SSH Configuration:</h2>
The console cable is disconnected from the Admin PC to Switch 1. The PCs command prompt is used to connect to the switch via SSH. A password is requested upon attempt, and a banner is displayed. The password for the "enable" feature is also prompted: <br/>
<img src="https://imagizer.imageshack.com/img923/2866/FdOg6v.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
