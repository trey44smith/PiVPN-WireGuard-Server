<h1>Raspberry Pi VPN with WireGuard</h1>

 ### [YouTube Demonstration](https://youtube.com/shorts/Nn0q-shzJ7I)

<h2>Description</h2>
<b>Installing my own personal Raspberry Pi-based VPN into my network using PiVPN and WireGuard in order to access my local servers and files when away form home. </b>
<br />

<h2>Architecture</h2>
<img src="https://i.imgur.com/kkp5lpc.png" height="80%" width="80%" alt="install the OS onto the Pi"/>
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
Confirm the Settings:  <br/>
<img src="https://i.imgur.com/glVpGuQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
Choose the Local User:  <br/>
<img src="https://i.imgur.com/P0ReoiT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
Choose WireGuard as the VPN software:  <br/>
<img src="https://i.imgur.com/cMhiYLL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
 Select and Confirm the WireGuard Port Number:  <br/>
<img src="https://i.imgur.com/nCJRZuz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <img src="https://i.imgur.com/AmWdxCI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
 Select CloudFlare for DNS Resolution:  <br/>
<img src="https://i.imgur.com/0TYbkAs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <br />
 Enable Security Patches and Reboot:  <br/>
<img src="https://i.imgur.com/d7k376u.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <img src="https://i.imgur.com/Cy61Jke.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <img src="https://i.imgur.com/VqUVSGA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <img src="https://i.imgur.com/duFKVWt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <br />
 Add users:  <br/>
 <code> pivpn -a</code>
 <br />
 <img src="https://i.imgur.com/LgG9QFy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <br />
 Enable Port Forwarding in the Firewall:  <br/>
<img src="https://i.imgur.com/UJAZ1Tk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <br />
 Download the WireGuard App and Connect Mobile Devices via QR Code:  <br/>
<code> pivpn -qr</code>
 <br />
 <img src="https://i.imgur.com/xdVsqde.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <br />
 Connect Your Laptop using FileZilla to connect to the Raspberry Pi and Download the config file:  <br/>
<img src="https://i.imgur.com/4AUtjNs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <br />
 Click the Import Tunnel(s) from File Button in the WireGuard App:  <br/>
<img src="https://i.imgur.com/d8ZLvDs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
 <br />
 Tunnel is Created:  <br/>
<img src="https://i.imgur.com/SK30Yx9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
 <br />
<br />
<br />
 Backup the PiVPN Server:  <br/>
<code> pivpn -bk </code>
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
