# IcedID_Lab_solution


This is a solution guide for the IcedID Lab in CyberDefenders.


Q1 

What is the name of the file associated with the given hash?

Answer

Firstly, you download the file from CyberDefenders and extract the hash value.
After that, you go to the VirusTotal website (https://www.virustotal.com/gui/home/upload) and you search for that specific hash value.
Once you've done that, you go to the "details" tab, scroll down to names, and there you can see the name of the file, which is "document-1982481273.xlsm"

Q2

Can you identify the filename of the GIF file that was deployed?

Answer

To solve this, go to the "Behavior" tab, scroll down until you see "Files dropped," and you will see that the program drops some files to specific locations on the hard drive.
You can see the names of files, and we know that we are looking for a .GIF file. So the file we're looking for is "3003.gif"

Q3

How many domains does the malware look to download the additional payload file in Q2?

Answer

To solve this question, simply go to the "Relations" tab, and from there, you can view the contacted URLs.
Then, simply count the number of URLs that contain the 3003.gif file. That number is 5.

Q4  

From the domains mentioned in Q3, a DNS registrar was predominantly used by the threat actor to host their harmful content, enabling the malware's functionality. 
Can you specify the Registrar INC?

Answer

To solve this question, simply compare the contacted URLs section to the Contacted Domains section. 
From there, you can understand that 3 URLs do not have Registar and the 4th provides a 404 message (meaning there is nothing in that ULR).
So the correct Registrar is "NAMECHEAP".


Q5

Could you specify the threat actor linked to the sample provided?

Answer

To solve this question, you need to go to the "https://attack.mitre.org/" website.
There, you can search the IcedID.Click the first result, and then scroll down until you find "Groups That Use This Software" section, and then click the first ID.
There, you can see the name of the thread actor is GOLD CABIN

Q6

In the Execution phase, what function does the malware employ to fetch extra payloads onto the system?

Answer

To solve this question, you need to go to the "behavioral" tab and expand the "MITRE ATT&CK Tactics and Techniques" and find the "execution" sector.
Inside there, you can find a function called "URLDownloadToFileA".




