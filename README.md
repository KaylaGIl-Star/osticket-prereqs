<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


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
- Set-up osTicket in browser

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

<h2>3.PHP Stack Prepared </h2>
<p>
<img width="1120" height="808" alt="Screen Shot 2025-12-16 at 11 58 11 AM" src="https://github.com/user-attachments/assets/6edc751a-c631-4f92-95c8-9e9364edcaf8" /><p>
  <img width="1540" height="808" alt="Screen Shot 2025-12-16 at 12 40 55 PM" src="https://github.com/user-attachments/assets/5b9d4f4a-6b22-4e5c-8540-2ab2f3bbb5a5" />
  <img width="1901" height="1130" alt="Screen Shot 2025-12-16 at 12 07 52 PM" src="https://github.com/user-attachments/assets/f54ddf6f-a086-4d1b-bb5d-938d2398a28c" />
<P> C:\PHP directory created → PHP 7.3.8 ready to extract into C:\PHP → Installers prepared (PHP Manager for IIS → URL Rewrite Module → VC_redist.x86) → Application installers ready (MySQL 5.5.62 → osTicket v1.15.8 → HeidiSQL).</p>
<br />

<h2>4. MySQL + osTicket files ready </h2>
<p><img width="1119" height="803" alt="Screen Shot 2025-12-16 at 12 02 24 PM" src="https://github.com/user-attachments/assets/4070955d-b3aa-4cfd-b07f-2ff101e7aba1" /></p>
<p><img width="1886" height="1008" alt="Screen Shot 2025-12-16 at 12 30 06 PM" src="https://github.com/user-attachments/assets/c2350c67-5234-4986-ae0e-5e6fbb86b2c4" /></p>

Unzip osTicket → Copy upload to C:\inetpub\wwwroot → Rename to osTicket → Restart IIS → Browse site → Enable PHP extensions (imap, intl, opcache) → Rename ost-sampleconfig.php to ost-config.php → Set permissions: Everyone → Full Control.

<h2>5. Set-up osTicket in browser </h2>
<img width="1590" height="893" alt="Screen Shot 2025-12-16 at 12 44 46 PM" src="https://github.com/user-attachments/assets/e5109352-c7c7-45a5-bef8-f0f0f2bc813e" />
<img width="955" height="760" alt="Screen Shot 2025-12-16 at 12 47 34 PM" src="https://github.com/user-attachments/assets/c4ed5e63-34be-4434-b972-6765a949248b" />
<img width="1552" height="983" alt="Screen Shot 2025-12-16 at 12 58 43 PM" src="https://github.com/user-attachments/assets/69b3d055-e4cc-472a-89b6-e80a8914bf7b" />
<img width="1575" height="1006" alt="Screen Shot 2025-12-16 at 1 02 19 PM" src="https://github.com/user-attachments/assets/5e0ca088-7553-429e-9b38-1f3a01f5b586" />

Click Continue → Enter helpdesk name + default email → Install & open HeidiSQL → Connect (root/root) → Create osTicket database → Enter DB details in browser → Click Install Now → Verify admin login
