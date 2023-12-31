# File-permissions-Linux

<h2>Description</h2>
This project explores Linux permissions. I go through the initial permissions and provide changes based on need. I also provided detail on why some of the changes were needed. There are many ways to make certain changes, so my examples are not finite. 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Bash</b> 

<h2>Environments Used </h2>

- <b>Linux</b> 

<h2>Program walk-through:</h2>

<p align="left">
Check file and directory details: <br/>
<img src="https://i.imgur.com/IKfKvXS.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Describe the permissions string:<br />
I will describe project_k.txt. <br />

* The first space determines if the file type is either d= directory or - = regular file. 
* The next three spaces identify user permissions: r (read) & w(write). 
* The first spot for you is “-” meaning no x(execute) permissions. 
* The next three slots are for group permissions. 
* Again, the group has r (read) & w(write)but no x(execute).
* The last three slots are for other permissions. Just as before, the group has r (read) & w(write)but no x(execute)
<br />
<br />
Change file permissions:<br/>
Others cannot have access to write in this database we must remove w(write) from other. The file that has this contradiction is project_k.txt. Below, you can see the code used to remove w.<br/>
<img src="https://i.imgur.com/GSK9yyX.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Change file permissions on a hidden file<br/>
The research team has archived .project_x.txt, so it’s a hidden file. This file should not have write permissions for anyone, but the user and group should be able to read the file. Below I have provided a screenshot showing the permission on the file to r(read) only<br/>
<img src="https://i.imgur.com/G8qGQqV.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Change directory permissions:  <br/>
The files and directories in the projects directory belong to the researcher2 user. Only researcher2 should be allowed to access the drafts directory and its contents. Below you can see the code used to remove access from drafts to anyone but user. <br/>
<img src="https://i.imgur.com/XQFzOno.jpg" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Summary:  <br/>
Being able to manage permission in Linux is important for security. As seen above, people can have access to documents they should not, which compromises document integrity.  By keeping up to date with permission changes, the company can better secure its information and stakeholders.
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
