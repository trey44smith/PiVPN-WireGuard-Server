<h1>Raspberry Pi VPN with WireGuard</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Description</h2>
<b>Installing my own personal Raspberry Pi-based VPN into my network using PiVPN and WireGuard in order to access my local servers and files when away form home. </b>
<br />


<h2>Utilities Used</h2>

- <b>Raspberry Pi 4</b> 
- <b>Port Forwarding</b> 
- <b>SSH</b>
- <b>VPN</b>

<h2>Environments Used</h2>

- <b>Raspberry Pi OS Lite (32-bit)</b>

<h2>Program walk-through:</h2>

<p align="center">
Install the OS: <br/>
<img src="https://imgur.com/PFKqdz8.jpg" height="80%" width="80%" alt="install the OS onto the Pi"/>
<br />
<br />
Edit the Settings:  <br/>
<img src="https://imgur.com/DFMQGL4.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enable SSH: <br/>
<img src="https://imgur.com/gDSJe2g.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Save Settings and Ensure OS Write is Successful:  <br/>
<img src="https://imgur.com/Ho6pYSE.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
SSH into Raspberry Pi:  <br/>
<img src="https://imgur.com/epm8v2Y.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Update the Raspberry Pi using the Terminal:  <br/>
 <code> sudo apt update && sudo apt upgrade  </code>
<br />
 <br />
Install PiVPN using the Terminal:  <br/>
 <code> curl -L https://install.pivpn.io | bash  </code>
<br />
 <br />
This will start the PiVPN installation wizard:  <br/>
<img src="https://i.imgur.com/x1uPM1h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
This will start the PiVPN installation wizard:  <br/>
<img src="https://i.imgur.com/x1uPM1h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Set a Static IP on the PiVPN Server:  <br/>
<img src="https://i.imgur.com/l6dl61Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
Edit the Settings:  <br/>
<img src="https://imgur.com/DFMQGL4.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
 Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
 Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
 Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
 Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
