<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 11</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Windows VM created and accessible
- IIS installed with CGI enabled on the VM.
- PHP stack prepared
- MySQL + osTicket files ready
- Item 5

<h2>Installation Steps</h2>


<h2>1.Azure Windows VM created and accessible</h2>
<p>
<img width="1953" height="1298" alt="Screen Shot 2025-12-10 at 2 36 08 PM" src="https://github.com/user-attachments/assets/de1d1708-25c1-4f53-91cc-0cd8dbff3d6b" /> </p> 
<p><img width="1085" height="415" alt="Screen Shot 2025-12-10 at 2 45 18 PM" src="https://github.com/user-attachments/assets/51366625-38b6-4239-a10c-798c0084558f" />
</p>
<p><img width="931" height="650" alt="Screen Shot 2025-12-10 at 3 01 05 PM" src="https://github.com/user-attachments/assets/c6a2889e-2129-4aa0-b189-e3e0f95af542" />
</p>
<p><img width="1635" height="950" alt="Screen Shot 2025-12-10 at 3 18 05 PM" src="https://github.com/user-attachments/assets/ee910559-f8d6-47a8-8a9e-4f89d42c4dd6" /></p>

Azure Portal →  Create → Azure virtual machine →
Select Subscription → Select Resource Group → Name the VM → Choose Region →
Choose Image (Windows/Linux) → Choose Size → Select Authentication Type →
Set Username/Password or Upload SSH Key → Next: Networking →
Ensure Public IP is enabled → Add inbound rule (RDP 3389 or SSH 22) →
Review + Create → Create.

<h2>2. Install/ Enable Internet Information Services in Windows With Common Gateway Interface</h2>

<p><img width="1150" height="642" alt="Screen Shot 2025-12-10 at 3 39 15 PM" src="https://github.com/user-attachments/assets/7a1342f6-dd90-47fc-b308-984f335af83c" />
</p>
Control Panel → Programs → Turn Windows features on or off →
Check “Internet Information Services” →
Expand it →
Expand “World Wide Web Services” →
Expand “Application Development Features” →
Check “CGI”.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
