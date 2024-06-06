<h1> Created a systemd Startup Script (Linux) </h1>

<h2>Description</h2>
This project involves creating and implementing a systemd startup script on an Ubuntu system. The script will automate the task of checking disk space usage and logging the output to a file. The steps include checking if MySQL is running, creating a systemd service file, writing a shell script to perform the disk check, setting appropriate permissions, and managing the service using systemd commands.

<h2>Languages and Utilities Used</h2>

- <b> Operating System: Ubuntu Server </b>
- <b> Linux Command-Line Tools: df, date, chmod, systemctl </b>
- <b> VCASTLE </b>
- <b> Bash Scripting: df-check.sh </b>
- <b> Systemd: df-check.service </b>
- <b> Text Editors: nano </b>

<h2>Screenshots:</h2>

<p align="center">
MySQL Check: <br/>
<img src="https://i.imgur.com/KynBRd3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created a df-check.service file in /etc/systemd/system:  <br/>
<img src="https://i.imgur.com/SJKkav1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created a shell script in /usr/local/bin that displays the disk free statistics (df -h) for system, date, and sends the output to a /root/df_report.txt file: <br/>
<img src="https://i.imgur.com/DnjroWG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
I adjusted permissions, reloaded systemctl, enabled and started the df-check service, checked the report, then stopped and disabled the service.:  <br/>
<img src="https://i.imgur.com/MdHNDc6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
