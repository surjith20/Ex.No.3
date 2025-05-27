# 19CS545-Ex3 - Create users, groups and group memberships in GitHub

# AIM:
To create users, groups and group memberships.
# Procedure:
1. Crea ng a group 
The first line [root@serverb ~]# groupadd admin creates a new group named 
admin. A group is a collec on of users that can share certain permissions. The root user is the 
system administrator and has the authority to create groups. 
2. Adding users to the group 
The next three lines [root@serverb ~]# useradd -G admin harry, 
[root@serverb ~]# useradd -G admin natasha, and [root@serverb 
~]# useradd -G admin sarah create three new user accounts named harry, 
natasha, and sarah. The useradd command is used to create new user accounts. The -G 
admin op on adds the new user to the admin group that was previously created. 
3. Se ng a restricted shell for a user 
The line [root@serverb ~]# useradd -s /sbin/nologin sarah creates a 
new user account named sarah. However, the -s /sbin/nologin op on specifies that the 
user's shell is set to /sbin/nologin. This is a special shell that restricts the user from logging 
into the system using a standard login method. Users with this shell can only be granted access 
through special means. 
4. Changing passwords 
The lines [root@serverb ~]# passwd repeated three mes ini ates a password change 
for the users harry, natasha, and sarah respec vely. The passwd command is used to 
change a user's password. 
Since the user execu ng the commands is root, they are able to change passwords for other 
users on the system. In a normal user account scenario, you would only be able to change your 
own password using this command. 
The text following passwd: prompts the user for the new password. For security purposes, the 
characters typed are not shown on the screen. 
5. Verifying password change 
 5
The line stdin harry (and similarly for natasha and sarah) shows that the user has 
successfully entered a new password. 
The line all authentication tokens updated successfully. following each 
password change indicates that the system has updated all login creden als associated with the 
user account.

# Output:
![image](https://github.com/user-attachments/assets/7bf6e572-6eac-4f57-9b1c-28b8b1203164)

# Result:
Thus the users and groups are created successfully. 
