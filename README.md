# Ransomware Demo

## Background and Disclosure
The purpose of this lab is to demonstrate a foundational understanding of ransomware, how ransomware is written, executed, and how threat actors extort countless victim organizations every year. This demonstration was done in a virtual machine operated by me alone and was not distributed outside of the virtual machine. This demo is meant for educational and informational purposes only, and is not meant to encourage or instruct others to take this information and use it for harmful purposes.<br />
<br />
The progress of this lab is outlined in the Description and displayed in the Screenshots sections below.

## Description
- Set up a virtual machine for testing a ransomware program run in Windows Visual Studio 2022.
- Downloaded a variety of files to different locations within the virtual machine to demonstrate that select folders can be targeted based on content, sensitivity, and value of the information.
- Configured a C# ransomware template to meet custom parameters. This demonstrates how the malware is written from the perspective of a threat actor.
- Encrypted the Documents, Pictures, and Desktop folders, and left a ransom note. This demonstrates what a real ransomware incident would look like from the perspective of a victim.
- Decrypted the affected folders, simulating what a vcitim would see after a ransom is paid.
- Located the executable files for this project to show that it could theoretically be shared with others or installed on other machines.

## Skills Learned
- Ransomware Functionality & Propogation
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
Figure 3: Once encryption has begun, this is what the scientist would see in real time. Notice the encrypted files are not able to be viewed as before, and have a new file extension (jcrypt). This file extension is what will tell the decryption program what files to target if the ransom is paid. 
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Encryption%20In%20Progress.PNG"/> <br />
<br />
<p align="center">
Figure 4: Logs sent in the body and as an attachment to the email.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%204.%20Logs%20Sent%20In%20Body%20of%20Email%20And%20As%20Attacment.PNG"/> <br />
<br />
<p align="center">
Figure 5: By modifying the Output Type, the keylogger will run discretely in the background.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%204.%20Configured%20OutPut%20Type.PNG"/> <br />
<br />
<p align="center">
Figure 6: Example of the keylogger harvesting login credentials on a banking website.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%206.%20Sample%20Login%20Banking%20Capture.PNG"/> <br />
<br />
<p align="center">
Figure 7: The same harvested credentials from Figure 6 are emailed to the test email address.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%207.%20Sample%20Credentials%20Sent%20To%20Test%20Email.PNG"/> <br />
<br />
<p align="center">
Figure 8: Keylogger executeable file shown in File Explorer that could theoretically be shared with others or installed on other machines.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%208.%20Shareable%20File%20With%20Custom%20Code.PNG"/> <br />
<br />
<p align="center">
Figure 9: Task setup to automatically start the keylogger in the background upon user logon.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%209.%20Task%20Scheduler%20Main%20Page.PNG"/> <br />
<br />
<p align="center">
Figure 10: Task Scheduler view showing the trigger and the action of the keylogger task.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%2010.%20Task%20Scheduler%20Trigger%20and%20Action.PNG"/> <br />
<br />
<p align="center">
Figure 11: Defender blocking the keylogger from running.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%2011.%20Defender%20Blocking%20Keylogger%20Execution.PNG"/> <br />
<br />
<p align="center">
Figure 12: Keylogger quarantined by Defender.
<img src="https://github.com/bryanotoole/Project-Pictures/blob/main/Keylogger%20Demo%2012.%20Defender%20Blocked%20Keylogger%20Executeable.PNG"/> <br />
<br />
