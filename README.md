<h1>Ransomware Attack on VMware using Kali</h1>

<h2>Description</h2>
The project consists of a simple procedure of attacking a client using Ransomware. The specific malware deployed in this lab is WannaCry. Recall that Ransomware is an example of malware where the attacker’s request payment with a threat. The attacker can hide/encrypt all or part of the victim’s file system and request payment to get access back to the encrypted files. The attacker can threaten to release the victim’s data to the public if they don’t pay. 
<br />

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
1.	Connect Kali to NAT
2.	In the Kali Linux, open a Terminal
3.	Type hostname -I to retrieve the IP address of the Linux
<br/>
<img src="https://imgur.com/a/ycl7MiT" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
  
Select the disk:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
