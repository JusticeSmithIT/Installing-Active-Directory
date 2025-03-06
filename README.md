<h1>AD - Installing Active Directory</h1>



<h2>Description</h2>
Project demonstrates how to install Active Directory Users and Computers using Server Manager in Windows 2022 VM. This allows the user the ability to create a domain controller and access features under that domain controller. Some of these features include, creating new users, organizational units, and enabling/disabling accounts.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Server Manager</b> 
- <b>Active Directory</b>

<h2>Environments Used </h2>

- <b>Windows 2022</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Launch Server Manager: <br/>
  
![image](https://github.com/user-attachments/assets/93531a7f-87e0-4b22-ac14-b85ac5b9f9b4)

<br />
<br />
Click "Add roles and features":  <br/>

![image](https://github.com/user-attachments/assets/66310393-f1d1-4334-b6d9-072e537d9d08)

<br />
<br />
Select Destination Server: <br/>

![image](https://github.com/user-attachments/assets/98e70625-650c-4ede-bd93-6e07ea528c9f)

<br />
<br />
Confirm and Install:  <br/>

![image](https://github.com/user-attachments/assets/6c98c901-9f05-4c60-9553-dad79507bf20)

<br />
<br />
Install done:  <br/>

![image](https://github.com/user-attachments/assets/1ba67af2-db7b-4a79-b59c-6bd36904c4ca)

<br />
<br />
Select flag Icon and "Promote this server to a domain controller":  <br/>

![image](https://github.com/user-attachments/assets/7fd909ef-4905-40a0-951f-2efc5d91a83d)

<br />
<br />
Add a new Forest:  <br/>

![image](https://github.com/user-attachments/assets/3ae77454-f257-4d18-bc35-ed8c4c7eb549)

Domain Controller is now Configured:  <br/>

![image](https://github.com/user-attachments/assets/03efb45f-24dd-4e93-8047-b1a0ef4b425b)



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
