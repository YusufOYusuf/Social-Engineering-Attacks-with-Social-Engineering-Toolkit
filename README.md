<h1>Social Engineering Attacks with Social Engineering Toolkit</h1>


<h2>Description</h2>
In this lab I learned to use The SET toolkit or “Social Engineering Toolkit”. This is an effective prepackaged toolkit for performing reconnaissance against a target. This lab demonstrates the use of some of its available attacks.
<br />



<h2>Environments Used </h2>

- <b>Kali GNU/Linux (2.0) sana 64-bit</b> 

<h2>Program walk-through:</h2>

<p align="center">
Open a new terminal by clicking on the Terminal icon located on the left panel.: <br/>
<img src="https://i.postimg.cc/DZ98fTDQ/Screen-Shot-2022-09-10-at-8-01-38-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
<br />
Type the command "setoolkit" followed by pressing Enter to open the Social Engineering Toolkit.:  <br/>
<img src="https://i.postimg.cc/zfL8mGGq/Screen-Shot-2022-09-11-at-4-29-40-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
When notified that SET is outdated, press the Enter key to continue : <br/>
<img src="https://i.postimg.cc/9MLySb84/Screen-Shot-2022-09-11-at-4-32-52-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  

  
  
  
<br />
Read through the Terms of Service and press the Y key followed by pressing Enter to continue.:  <br/>
<img src="https://i.postimg.cc/9MLySb84/Screen-Shot-2022-09-11-at-4-32-52-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
 
 
 
 
 
 
 <br />
On the SET main page, select the 1) Social-Engineering Attacks menu item by pressing 1 followed by pressing Enter.:  <br/>
<img src="https://i.postimg.cc/rF428P1L/Screen-Shot-2022-09-11-at-4-35-40-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
 
 
 
 
 
 
 
  
<br />
On the Social-Engineering Attacks page, select the 2) Website Attack Vectors menu item. Press 2 followed by pressing the Enter key.:  <br/>
<img src="https://i.postimg.cc/D0rVcWyw/Screen-Shot-2022-09-11-at-4-37-49-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
  
  
  
  
  
<br />
On the Website Attack Vectors page, select the 3) Credential Harvester Attack Method menu item. Press 3 followed by pressing the Enter key.:  <br/>
<img src="https://i.postimg.cc/mgqdtLBX/Screen-Shot-2022-09-11-at-4-42-45-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 
  
  
  
  
  
  
  
 <br />
On the Credential Harvester Attack Method page, select the 1) Web Templates menu item. Press 1 followed by pressing the Enter key.:  <br/>
<img src="https://i.postimg.cc/3NSXV1wS/Screen-Shot-2022-09-11-at-4-48-13-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 
   
  
  
  
  
  
  
 <br />
When prompted for an IP address for the POST back, enter the IP address [192.168.9.2] of the Kali machine. Press Enter.:  <br/>
<img src="https://i.postimg.cc/RhN66BMd/Screen-Shot-2022-09-11-at-4-53-06-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 
  
  
  
  
  
  
  
  
  
  <br />
On the Select a template prompt, select the 2. Google menu item. Press 2 followed by pressing the Enter key.:  <br/>
<img src="https://i.postimg.cc/t40ZTw8d/Screen-Shot-2022-09-11-at-4-55-05-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 
  
  
  
  
  
  
<br />
When prompted for SET to start the Apache process, press Y followed by the Enter key to continue. :  <br/>
<img src="https://i.postimg.cc/TwBPzKb6/Screen-Shot-2022-09-11-at-5-01-56-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 
  
  
  
  
  

<br />
If your Kali webserver is not running, the tool will start it and copy all the necessary files to the /var/www directory. When prompted, press the Enter key to continue.:  <br/>
<img src="https://i.postimg.cc/rszPrpZK/Screen-Shot-2022-09-11-at-5-04-45-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 







<br />
Open a new Terminal by clicking the File tab and selecting Open Terminal.:  <br/>
<img src="https://i.postimg.cc/Hswh8FB0/Screen-Shot-2022-09-11-at-5-07-55-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>







<br />
Navigate to the /var/www/html directory by typing the command "cd /var/www/html". Press Enter.:  <br/>
<img src="https://i.postimg.cc/G3YM6Zw0/Screen-Shot-2022-09-11-at-5-10-02-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>






<br />
List the current files in the directory by using the command "ls -l":  <br/>
<img src="https://i.postimg.cc/2j4w0hhr/Screen-Shot-2022-09-11-at-5-11-49-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>








<br />
Edit the post.php file by typing the command "nano post.php". Press Enter:  <br/>
<img src="https://i.postimg.cc/4dv9QvM0/Screen-Shot-2022-09-11-at-5-14-02-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>







<br />
Using the arrow keys, move the cursor towards the end of the line. In the nano editor, change the return URL from url=http://www.google.com to url=http:192.168.9.2.:  <br/>
<img src="https://i.postimg.cc/FHGjJX8L/Screen-Shot-2022-09-11-at-5-19-38-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>





<br />
Once modified, press CTRL + X to exit. When prompted to save, press Y. When prompted for file name, press Enter to save as post.php.:  <br/>
<img src="https://i.postimg.cc/ht3XBDNp/Screen-Shot-2022-09-11-at-5-22-56-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>






<br />
Click on the Application Launcher icon located in the bottom left corner and select the Firefox icon to launch the web browser.:  <br/>
<img src="https://i.postimg.cc/W3TkX2K8/Screen-Shot-2022-09-11-at-5-29-19-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>






<br />
In the Firefox window, type 192.168.9.2 into the address bar. Press Enter.:  <br/>
<img src="https://i.postimg.cc/ZqsKG4D4/Screen-Shot-2022-09-11-at-5-31-04-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>






<br />
Enter email and password and sign in:  <br/>
<img src="https://i.postimg.cc/kG4Fvxhq/Screen-Shot-2022-09-11-at-5-36-21-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>






<br />
Navigate back to the Kali PC viewer. Focus on the Terminal window with /var/www/html as the current directory. Type the command "ls" to list the files in the directory.:  <br/>
<img src="https://i.postimg.cc/JhxkYsXn/Screen-Shot-2022-09-11-at-5-38-27-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 






<br />
Type the command "cat harvester_<rest of file name>" to view the contents of the harvester file. Do not type the text <rest of file name>...(Note that it is easier to use the Tab command completion feature in Linux. Type
cat harvester and then press the Tab key for the system to complete the
actual filename. Make sure to replace <rest of file name> with the dynamic
dated information in the harvester filename.):  <br/>
<img src="https://i.postimg.cc/zG0KDdz7/Screen-Shot-2022-09-11-at-5-44-25-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 







<br />
Notice the email and password have been obtained successfully.:  <br/>
<img src="https://i.postimg.cc/mg21nQYH/Screen-Shot-2022-09-11-at-5-46-09-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/> 















  
  
  
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
