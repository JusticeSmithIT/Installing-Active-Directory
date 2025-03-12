<h1>Installing Active Directory and Configuring Domain Controllers</h1>



<h2>Description</h2>
Project demonstrates how to install Active Directory Users and Computers using Server Manager in Windows 2022 VM. This allows the user the ability to create a domain controller and access features under that domain controller. Some of these features include, creating new users, organizational units, and enabling/disabling accounts.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Microsoft Azure</b>
- <b>Server Manager</b> 
- <b>Active Directory</b>
- <b> Windows Remote Desktop for MacOS</b>

<h2>Environments Used </h2>

- <b>Windows Server 2022</b> 

<h2>Program walk-through:</h2>

<p align="center">
Launch Server Manager, select "Add roles and Features": <br/>
  
![Screenshot 2025-03-06 at 12 15 47 PM](https://github.com/user-attachments/assets/357a89f6-f651-464c-ad7f-e16750c6e6bf)


<br />
<br />

Select Destination Server, which in this case it is "dc-1" and select "next.". <br/>

![image](https://github.com/user-attachments/assets/2cc83c3e-a2e1-40d8-9d4a-e6fdb9a4b859)


<br />
<br />


Once you get to this window, select "add features" and keep the box checked that says "include management tools," then click next. <br/>

![image](https://github.com/user-attachments/assets/dffcf0ad-4b60-4728-83de-56b6c1089638)



<br />
<br />


Confirm installation selections and allow automatic restarts. Check the box that shows "Restart the destination server automatically if required.":  <br/>

![image](https://github.com/user-attachments/assets/5dd63dae-f896-4116-9594-2524eb4b1b1e)


<br />
<br />
The Installation process will then start, wait a few moment for it to complete.   <br/>

![image](https://github.com/user-attachments/assets/531004d0-96d9-4ce2-9e68-c0bf0fa3a0fd)


<br />
<br />
The Installation process is now complete but we still must promote the server to a domain controller.  <br/>

![image](https://github.com/user-attachments/assets/3d022121-b499-4dc5-9a5a-04dca45f0af1)



<br />
<br />
Select the flag icon in the top right corner of the window and under "post deployment configuration" click "promote this server to a domain controller."  <br/>

![image](https://github.com/user-attachments/assets/c6e64233-be66-491b-903b-206844529efa)


In this window, select add a new forrest and name it "mydomain.com", then select next.  <br/>

![image](https://github.com/user-attachments/assets/8bd3b246-53f3-4a17-bff3-45d36ba38f16)

Under domain controller options, leave everything the way it is besides the password. Create a password and confirm it. This is the password for non-local users to log in with for the new domain.  <br/>

![image](https://github.com/user-attachments/assets/28fe485e-51c9-43a9-8a21-8d8941de4f3a)


Deselect the box, "create DNS delegation" and select next.  <br/>

![image](https://github.com/user-attachments/assets/546a348d-efbc-4818-8a13-68a26ef06572)

The Prerequisites check will take a few moments to finish.  <br/>

![image](https://github.com/user-attachments/assets/b9d48a8e-6ad4-47c0-9c1d-e2199443c9e4)

Installation will now begin, wait a few moments for completion.  <br/>

![image](https://github.com/user-attachments/assets/e59f6308-f7ae-4c72-889b-66156aa0051e)

As soon as the installation is complete, the computer will automatically restart.  <br/>

![image](https://github.com/user-attachments/assets/f1be1848-3da1-4696-9bb3-0dc7123ab0fe)

Log back in to dc-1 as your domain, in this case it is "mydomain.com\user." Once you are logged in, press the start button in the bottom left corner, and search for "active directory users and computers." If it shows up, then active directory has been properly installed.  <br/>

![image](https://github.com/user-attachments/assets/6d3bf3a7-6d7e-42cf-9b04-a24344a660c9)


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
