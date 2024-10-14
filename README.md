<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://pi-hole.github.io/graphics/Vortex/Vortex_Vertical_wordmark_darkmode.png">
    <source media="(prefers-color-scheme: light)" srcset="https://pi-hole.github.io/graphics/Vortex/Vortex_Vertical_wordmark_lightmode.png">
    <img src="https://pi-hole.github.io/graphics/Vortex/Vortex_Vertical_wordmark_lightmode.png" width="168" height="270" alt="Pi-hole website">
  </picture>
    <br>

<h1>Pi-Hole Installation and Configuration</h1>
This tutorial outlines the Installation and Configuration of Pi-Hole on a Rasberry Pi Model 4B.<br />


<h2>OverView</h2
To install a Pi-hole in your network, you’ll need to do the following things:

Configure a Raspberry Pi running Raspberry Pi OS.

Set up Pi-hole software on your Raspberry Pi.

Direct DNS queries on your network to your Raspberry Pi.

<h2>Operating Systems Used </h2>

- Rasberry Pi OS 

<h2>List of needed Items</h2>

Raspberry Pi

Suitable power supply

MicroSD card

Adapter to connect your microSD card with your usual computer

USB cable

For the initial SD card setup, you will need:

Another computer 

<h2>Rasberry Pi OS Install</h2>

<p>
Go to: https://www.raspberrypi.com/software/ and Download the Imager Software 
<img src="https://i.imgur.com/izQxZGU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<p>

Once Downloaded and Installed set the correct image for your device
<img src="https://i.imgur.com/Gg957DH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />
<p>
  And install
  
  -Once Finished eject the SD Card and plug it into the Raspberry Pi.
<img src="https://i.imgur.com/uXzaySp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Rasberry Pi update </h2>

Now the your Device is set up and powered on, open a Terminal panel
<img src="https://i.imgur.com/niIvCQz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<p>
copy and run the following command:  

```bash
sudo apt update && sudo apt upgrade
```
<img src="https://i.imgur.com/It3UMoq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
Once Complete reboot the Rasberry Pi

```bash
sudo reboot now
```
<img src="https://i.imgur.com/ZSUWGAd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<br />

<h2>Pi-Hole Installation </h2>
  Once Rebooted copy and run the following command

```
curl -sSL https://install.pi-hole.net | bash
```

<img src="https://i.imgur.com/YdxDnIm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  Follow the Set up 
<p>
<img src="https://i.imgur.com/gU8nj6n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  When you are picking your upstream DNS provider select Quad9, as it is a non-profit organization which operates a privacy-and-security focused, open DNS recursive service 

  Here is their link if you have any questions: https://quad9.net/

  Continue the installation to your own Logging Preferance
<img src="https://i.imgur.com/Kd7W5qy.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  Take note of the IP address, you will need to go to your router and make this static.

  You can copy the premade password and log into the web address or the Ip/admin. Or the next step we are going to change it!
<img src="https://i.imgur.com/9nxbgkv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Copy and run this command:

```bash
pihole -a -p
```

<img src="https://i.imgur.com/pOjI5id.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
Next we will make sure everthing is updated, copy and run this command
  
```bash
pihole -up
```

<img src="https://i.imgur.com/QYUn9Ov.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<h2>Firebog DNS list</h2>

<p>
Open a web page and go to your pihole web page, and log in.
  
  http://<IP_ADDPRESS_OF_YOUR_PI_HOLE>/admin/
<img src="https://i.imgur.com/rIKryND.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  Open another tap and go to https://firebog.net/
<img src="https://i.imgur.com/EiGFPQI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to the Addlist tab on the left hand side menu

  We will pasting the URL's from Fire bog into the Addresses bar
<img src="https://i.imgur.com/fLsNouD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Copy at least the Green (I will be including the Blue options) it is recommended to avoid the ones with lines through them as they may block the wrong things and break websites!
<img src="https://i.imgur.com/l3W2CxM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
  Copy, paste and add all sections you desire!
<img src="https://i.imgur.com/4xqgkAk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Step 1
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Step 1
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Step 1
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Step 1
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br /><p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Step 1
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
Step 1
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
