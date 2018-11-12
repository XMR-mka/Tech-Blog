# CIS 141 Technical Blog
**Maxwell Ka**

kamaxwell41@gmail.com / mka@sierracollege.edu

8PHVN-VYCHH-QKM76-CQM93-C37Y9

## About Me

My name is Maxwell Ka and I am a part-time Sierra College student.  I also work
part-time at a local Wireless Internet Service Provider in Grass Valley, where I
live.  During my free time, I liked spending time with my friends and with my
computer, which I already get to spend quite a lot of time with at work and school.


### Skill 1.1 - Prepare for Installation Requirements

### Warm-Up: How Many Computers Are In This Room? (V-129)

There are 32 student workstations in V-129. [32 Computers]
There are (almost certainly) x + 1 cellphones in the room at any one time, where x= the number of students present,
so each one of those counts as a computer (The one is for the professor). [33 + x computers]
There is 1 projector, 1 landline phone, and 1 workstation at the teacher's desk. [36 + x computers]

Therefore, unless I'm missing some, there are 36 + x computers, where x is the number of students present.

### 1.1 Objectives

- Determine hardware requirements and compatibility
	- 1 GHz + processor
	- 1 GB RAM for 32-bit, 2 for 64-bit
	- 16 GB (32-bit) or 20 GB (64-bit) minimum hard disk space
	- DirectX 9 + with WDDM 1.0 driver
	- 800 x 600 display

- Choose between an upgrade and a clean installation
	- Wipe & Load: Viable for all scenarios
	- In-Place Upgrade: Recommended for existing Windows 7/8/8.1 devices
	- Provisioning: For Windows 10 CYOD scenarios
- Determine appropriate editions according to device type
- Determine and create appropriate installation media

### Skill 1.1 Technical Blog Response

1. For this response I chose my personal laptop, so I am the primary user.

2. The machine's specifations are as follows: **Intel Core i7-5500U 2.40GHz CPU**,
**16 GB RAM**, **Intel HD Graphics 5500 Integrated GPU**, **DirectX 11.2**, and a
**1920x1080 display**.  This machine's specifications are more than ample to meet
the Windows 10 minimum requirements.

3. To upgrade the machine, I would opt for an in-place upgrade without use of any
Microsoft evaluation tools, as the machine was purchased with Windows 8.1 and
all of the software currently installed is compatible with Windows 10.  While there
may be some benefit to performing a full reinstallation, since it is a secondary
PC and relatively well-maintined, I do not believe it is worth the time and hassle.

4. I would install Windows 10 Professional on this machine.  This is due to all of
the added features in Windows 10 Pro, such as Bitlocker, Remote Desktop, and Client Hyper-V
that I would like to be able to utilize.


### 1.3 Warmup Activity

Mikrotik is a manufacturer of routing and wireless equipment for ISPs and enterprise, and over the past couple of months they have come under fire for a security vulnerability in their gear.  This vulnerability, which allows attackers to take advantage of Mikrotik's built-in packet sniffing capabilities, was patched by Mikrotik in April, but for one reason or another over 370,000 unpatched Mikrotik routers are still sitting out on the Internet. According to reports by Netlab 360, over 7,500 of those unpatched routers are being actively spied on, and ~239,000 have been turned into proxy client devices that continuously scan for more potential targets.  Interestingly enough, in one variant of the malware that attempts to mine cryptocurrency, the attacker seems to have accidentally blocked their own external web resources from being reached via an Access Control List, rendering the malware useless in mining.  <https://arstechnica.com/information-technology/2018/09/unpatched-routers-being-used-to-build-vast-proxy-army-spy-on-networks/>

### Skill 1.2 Technical Blog Response

1. The Media Creation Tool is similar to the DIY USB installation in that both processes involve using a software image to install the operating system.  A key difference between the two is that while a USB drive is physical media you must plug in to your machine and boot it from, the Windows Media image is just a file you mount to your drive.

2. A user might want to have multiple partitions on a hard drive for many reasons, such as the ability to run multiple different operating systems on the same machine, or have different users use a different partition.  I took the following steps to create multiple partitions in my hard drive:
	- opened up "run"
	- opened up "diskmgmt.msc" via run
	- left-clicked NTFS segment of disk and "shrank volume" by 10 GB
	- left-clicked new 10 GB of unallocated disk space and chose "New Simple Volume" and answered all the prompts.
	- Voila, new partition!

3. *Describe each step that requires "user attention" during the clean installation of Windows 10*
	- Where you want to install Windows - If you select the wrong drive, you'll be stuck using the wrong drive for the rest of your installation, or be forced to start again (For example, if you wanted to install your OS on an M.2 drive instead of your HDD)
	- Region - If you select an incorrect region, many system settings will be inaccurate   
	- User - If you don't create a user with a password or use a Microsoft account, your installation may not be secure
	- Privacy - Allows you to tailor what information you share and do not share.

4. One Windows feature I chose to install after installation is SNMP, I did this by opening up "optionalfeatures.exe" in Run, and then choosing SNMP's box before pressing install.

### Sep. 17 Warmup Activity

*What is Patch Tuesday?  When did it last occur?  What was included in the most recent event?*
- Patch Tuesday is a term used to refer to the day that Microsoft regularly releases security patches for its software.  It regularly occurs on the second and sometimes fourth Tuesday of each month in North America, so the last Patch Tuesday was on September 11.  The patch included at least 61 different vulnerability fixes, mostly in Internet Explorer and Edge.  

### Skill 1.2 Technical Blog Response - Windows 8.1 Upgrade

1. *On Windows 8.1, install an application that may not be Windows 10 compatible.  Why do you think it may not be compatible?*
	- I installed paint.net, I believe it may not be compatible with Windows 10 as it was popularly used with Windows 8.1 and may not have been updated for the newest operating system.
2. *On Windows 8.1, create a very special text file.  What does it contain?  Where is it?*
	- The file contains the answer to life's greatest question.  It is located at C:\Users\Maxwell Ka\Documents.
3. *During the in-place upgrade to Windows 10, describe the steps that require user attention*
	- Get important updates: Choose whether to download most recent updates now, or wait til later to update.
	- Ready to Install / What to Keep: Keep everything, personal files only, or semi-clean wipe.
	- Privacy: Choose what information gets shared with Microsoft and other parties
4. *In what ways was the upgrade process similar to a clean installation?  How did it differ?*
	- In both processes, users must pay careful attention to ensure they select the right options for their install/upgrade.  Both processes also allow you to configure your privacy.
	- The processes differ in that the in-place upgrade requires much less configuration on the part of the user
5. *Are there additional folders that remain after the install process is complete?  What are the contents of those folders?*
	- The windows.old folder remains, it contains the files necessary to revert to the previous OS version.  

### Skill 1.3 Technical Blog Response

1. *Create a list of hardware that a user might have that requires a driver installation*
		- Mouse, Keyboard, Scanner, Printer, Headset, Wireless Adapter, external disc reader
2. *Locate a device from your list and install it on Windows 10*
		- I installed an Alfa Wireless 802.11ac wireless adapter.
3. *Locate the version of the driver and see if it is the most current version available*
		- It was not the most current version of the driver, [so I updated it](https://imgur.com/a/D7t3dMb)
4. *Disable the device.  Does this affect Windows performance?  What happens when you disable other devices?  Try disabling your network card - how was that experience?*
		- When I disabled the device, it did not affect windows performance as I have another wireless adapter in my laptop.
5. *Why would I disable updates over metered connections?  Capture a screenshot of where you disabled this feature*
		- I would disable updates over metered connections if I was using a connection that had limited data. [I did this here](https://imgur.com/a/KRLa2G7)
6. *Perform a rollback of a driver update.  Note, you will need to access a different USB device if you have been working with a printer*
		- [I did it](https://imgur.com/a/T0kEoVq)
7. *After installing a USB microphone, a system has extremely poor performance.  How would you check to see if the performance issues are related to the USB microphone?*
		- I would first check by rolling back the drivers for the USB microphone and removing the device, and seeing if that resolves any performance issues

### Skill 1.4 Technical Blog Response

1. *Using your textbook, ITPro.tv videos and notes, as well as Microsoft documentation, research one of the following post-installation activities, create a step-by-step guide, and test out your guide on your VM*
		- Configure and Customize the user interface per device type
		- Configure accessibility options
		- Configure Cortana
		- Configure Microsoft Edge
		- Configure Microsoft Internet Explorer
		- Configure Hyper-V
		- *Configure Power settings*
			1. Navigate to Power & Sleep in System settings
			2. Configure duration to turn off screen after when on battery power
			3. Configure duration to turn off screen after when charging
			4. Configure duration to sleep after when on battery power
			5. Configure duration to sleep after when charing
			6. To the right of the screen, click "Additional power settings"
			7. Configure what the power button does
			8. Configure what closing the lid does
			9. Create a power plan

### Skill 1.5 Technical Blog response

1. *Skill 1.5 Warmup - What is "UAC"? Why is it important?  When did Microsoft introduce UAC?  Is UAC on your Sierra Host machine different than your VM? If so, how so?*
    - UAC is User Access Control, and it is important because it allows a user to run less programs with privileged access, as well as be more productive when privileged access is not required.  Microsoft introduced UAC with the Windows Vista and Windows Server 2008 editions.  The UAC on my Sierra Host machine is nearly identical to that of the VM.

2. *Skill 1.5 Notes*
		-	LSDO: Local, Site, Domain, Organizational units - order of operations for user privileges in an enterprise environment
		- Group Policy
		 	- Local Group Policy Editor on Windows 10
				- Centralized Control for:
					- User settings
					- Computer settings
					- Control and Deployment of Applications
					- Control User Experience
			- What does it change?
			- gpupdate /force OR log off to apply Group Policy changes.
		- GPEdit Challenge
			- Can you:
				- *Block all Microsoft accounts?*
					- Computer configuration -> Windows Settings -> Security Settings - >
					Local Policies -> Security Options -> Accounts:Block Microsoft Accounts
				- *Enforce a password length of 10 characters?*
					- Computer configuration -> Windows Settings -> Security Settings - >
					Account Policies -> Password Policies -> Minimum password length
				- *Disable secure desktop in UAC?*
					- Computer configuration -> Windows Settings -> Security Settings - >
					Local Policies -> Security Options -> User Account Control: Switch to
					the secure desktop when prompting for elevation

### October 8 Warmup response

1. *What is a software bug? Describe the bug that is delaying the release of the 1809 update for Windows 10?*
		- A software bug is a flaw in software that causes it to behave in an unwanted or unexpected manner.  The bug in particular that is delaying the release of Microsoft's 1809 update is one that can cause user file deletion, as well as other minor issues such as incorrect CPU utilization metrics or broken audio drivers.

### Skill 2.1 Technical Blog Response

*Create a "Top 5" list of Windows 10 networking best practices, tips, tricks and troubleshooting strategies*

1. ipconfig /all - This command within command prompt displays the full information for all network adapters, and is a fantastic troubleshooting tool when looking for a host's network configuration. [Microsoft Doc](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/ipconfig)
2. tracert [insert host IP address] - This command within command prompt uses ICMP to trace the destination to the host, and is hugely helpful in identifying network communication and routing issues.  [Microsoft Doc](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/tracert)
3. ping [insert host IP address] - This command within command prompt uses ICMP to test connectivity to a single device, as well as verifying TCP/IP functionality in the host machine when used in combination with a loopback address.  [Microsoft Doc](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/ping)
4. When troubleshooting network issues, disabling and re-enabling the network adapter can often solve the issue, especially with older hardware.
5. nslookup - This utility within command prompt can be used to test and troubleshoot DNS, including viewing DNS information or changing name servers.  [Microsoft Doc](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/nslookup)

### Skill 2.2 Technical Blog Response

1. *You have a new desktop running Windows 10.  However, you try to copy your file repository and find out that you do not have enough disk space.  You have 400 GB of free disk space on your C drive and you have 3 smaller 500 GB drives.  What can you do?*
	- I could combine all of the drives into one large spanned volume using Disk Management.  This would provide enough storage to copy my file repository over

2. *You create a new storage pool for the following disks on your Windows 10 computer: 1 TB SATA, 1 TB SAS.  SATA and SAS are two different types of drives with different connectors and interfaces.  What is the maximum size you can allocate for your new storage space?*
	- The maximum size I can allocate for the new storage space is 2 TB, which would be with both of the 1 TB drives.  Storage Spaces allows you to pool the storage of different drives, regardless of connectors or interfaces.

### Skill 2.3 Technical Blog Response

Lab 09: Installing a Virtual Printer

1. *How many printer devices are installed on this machine?*
 - 3 
2. *How many printing devices are now displayed in the Devices and Printers window?*
 - 4
3. *What is the title of the new window that has appeared?*
 - Save print output as
4. *What extension is placed on the Printed File document now saved on the desktop?*
 - .prn
5. *Besides the original types message, what else is displayed in this Printed File?*
 - The title and the page number
6. *Which device has become the default printer now that the Virtual Printer has been*
removed?
 - Microsoft Print to PDF

Lab 10: Share a Virtual Printer

1. *How many printer devices are installed on this machine?*
 - 3
2. *How many printing devices are now displayed in the Devices and Printers window?*
 - 4
3. *What is now shown in the description at the bottom of the window?*
 - It shows that it is in a sharing state
4. *How many printer devices are installed on the PC1 machine?*
 - 3
5. *How many printers are now listed in the Devices and Printers window?*
 - 4
6. *What is the title of the window that opens?*
 - Save print output as
7. *Did the file appear on the desktop?*
 - Yes

Lab 12: Configure Local User File Sharing

1. *Which account type was created for the TEST user account?*
 - Standard User
2. *Who is the folder currently shared with?*
 - student
3. *Which three user accounts can this directory be shared with?*
 - student, Test, Everyone
4. *Which two accounts are now listed?*
 - Test and student
5. *What message appears?*
 - Access is denied
 
### October 29 Warmup

1. *Browse the Windows Store.  what app did you find that surprised you?  Is there an essential app to your life missing from the store?  What is it and where can one find it?*
	- I found a Bitcoin Miner app, which surprised me as most Mining applications are fairly non user-friendly, whereas this app is the opposite.
	- One app that is essential to my life that can't be found on the Microsoft store is Excel.  The only way to acquire Excel is to purchase a license for it (Or Microsoft office) from Microsoft or a distributor.  Nevermind, Excel is on the MS store, but at a huge markup compared to purchasing Office 2019 as a whole.

### Skill 2.4 Technical Blog Response

1. *You work for a small business of 25 employees, split between two offices that are in different buildings but share a parking lot.
You have been tasked with deploying Microsoft Office to all machines, Adobe CS Suite to the Marketing team, and QuickBooks to the Accounting Team.  You also want to allow users to selectively install Adobe Acrobat.
What would you do?*
	- I would use a Windows Provisioning Package and Windows Configuration Designer to distribute a single Windows Provisioning Package that includes Microsoft Office 2016, as well as a script to install it.  For Adobe CS Suite and QuickBooks I would again create a provisioning package and script to install the applications, then distribute them only to the appropriate departments.  To allow all users to selectively install Adobe Acrobat, I would use Configuration Manager to include Adobe Acrobat, and set it to be Available to users to install (Deployment Settings > Purpose > Available).
	
### Skill 2.5 Technical Blog Response

1. *Given the message (as shown above), of the three possible reasons listed, which one is
the most likely to be the cause of the remote connection failure?*
	- Remote access to the server is not enabled
2. *After the Remote Desktop successfully connects, what is displayed on the top of the
screen that identifies PC1 is being used?*
	- The IP address of PC1
3. *Why is it necessary to login to the PC1 machine again?*
	- Because PC2 made a change to the desktop
4. *Is the file created by PC2 on the desktop?*
	- Yes
5. *Joe is a new IT Director who is tasked with making sure his Windows 10 computer users can be assisted remotely. On his first day at the company, Joe was told that the Remote Assistance feature was not working for users after a new firewall was installed. What could be causing the problem and how should it be addressed?*
	- The firewall may be blocking the port for remote desktop protocol.  To fix this, one could try allowing the RDP port through the firewall.
6. *You are an administrator at the Contoso Corporation. You have a 12-person help desk that supports about 10,000 users spread out over a 5-building campus. You don’t have enough people to provide support staff visits to a user who is having problems. Describe the actions you can take to support your company users.*
	- I would provide support to the company users via Remote Desktop Connection, rather than visiting the staff in-person.  I could then provide the same level of support much more conveniently.  
