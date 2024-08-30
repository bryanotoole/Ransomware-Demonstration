# Ransomware Demo

## Background and Disclosure
The purpose of this lab is to demonstrate a foundational understanding of ransomware, how ransomware is written, executed, and how threat actors extort countless victim organizations every year. This demonstration was done in a virtual machine operated by me alone and was not distributed outside the virtual machine. This demo is meant for educational and informational purposes only and is not meant to encourage or instruct others to take this information and use it for harmful purposes.<br />
<br />
The progress of this lab is outlined in the Description and displayed in the Screenshots sections below.

## Description
- Set up a virtual machine to test a ransomware program run in Windows Visual Studio 2022.
- Downloaded a variety of files to different locations within the virtual machine to demonstrate that select folders can be targeted based on content, sensitivity, and value of the information.
- Configured a C# ransomware template to meet custom parameters. This demonstrates how the malware is written from the perspective of a threat actor.
- Encrypted the Documents, Pictures, and Desktop folders, and left a ransom note. This demonstrates what a real ransomware incident would look like from the perspective of a victim.
- Decrypted the affected folders, simulating what a victim would see after a ransom is paid.
- Located the executable files for this project to show that it could theoretically be shared with others or installed on other machines.

## Skills Learned
- Ransomware Functionality & Propagation
- C# Scripting

## Tools & Technology Used
- Oracle VirtualBox
- Microsoft Visual Studio 2022

## Screenshots

<p align="center">
Figure 1: Important files of the test user. The victim here being represented in this demo is an Iranian nuclear scientist. The scientist has a number of files on his Desktop that are of high value and secrecy, along with personal files in the Documents and Pictures folders. Losing access to these files without proper backup solutions would be detrimental.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Files%20Before%20Encryption.PNG"/> <br />
<br />
<p align="center">
Figure 2: Part of the C# code that makes up the ransomware. The parameters here direct the ransomware to target the Desktop, Documents, and Pcitures folers. The code also sets the password for decryoption, along with elements that will appear in the ransom message. <br/>
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Ransomware%20C%23%20Code.PNG"/> <br />
<br />
<p align="center">
Figure 3: Once encryption has begun, this is what the scientist would see in real time. Notice the encrypted files are not able to be viewed as before and have a new file extension (jcrypt). This file extension tells the decryption program what files to target if the ransom is paid.  
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Encryption%20In%20Progress.PNG"/> <br />
<br />
<p align="center">
Figure 4: Encryption is complete and the scientist's files are now unreadable. 
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Encryption%20Complete.PNG"/> <br />
<br />
<p align="center">
Figure 5: The scientist sees this message left by the threat actors asking for Bitcoin to be sent to the wallet address, along with a transaction ID emailed to the attackers. The wallet address, the amount of Bitcoin to send, and the email address were all defined in the C# code in Figure 2. 
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Ransom%20Message.PNG"/> <br />
<br />
<p align="center">
Figure 6: Less flashy ransom notes are sometimes left by threat actors like here in Figure 6. We can see the ransom instructions and what files were encrypted. Here, the attackers wished the victim a nice day. But it is in fact, NOT a nice day for the scientist.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Ransom%20Note%20Left%20On%20Desktop.PNG"/> <br />
<br />
<p align="center">
Figure 7: The decryption C# code is shown here. The parameters of the code target the jcrypt files on the victim's device.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Decryption%20C%23%20Code.PNG"/> <br />
<br />
<p align="center">
Figure 8: After paying the ransom, the scientist is given the decryption key so he can access his cat photos again.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Files%20Decrypted.PNG"/> <br />
<br />
<p align="center">
Figure 9: Like the ransom note, the decryption file generates a decryption log showing what files were decrypted.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Decryption%20Log.PNG"/> <br />
<br />
<p align="center">
Figure 10: Executable files shown in File Explorer that could theoretically be shared with others or installed on other machines.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Encrypter%20%26%20Decrypter%20Folders%20In%20Safe%20Area.PNG"/> <br />
<br />
