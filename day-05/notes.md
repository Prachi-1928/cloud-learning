\# Day 5 - Linux Users and Permissions



\## Linux Users

Linux is a multi-user operating system.



Common user types:

\- Root user

\- Regular user



\## Root User

The root user has complete administrative access to the system.



\## File Permissions



Linux permissions are divided into:



\- Read (r)

\- Write (w)

\- Execute (x)



Permissions apply to:

\- Owner

\- Group

\- Others



\## chmod

Used to change file permissions.



Example:



chmod 755 file.txt



\## Permission Numbers



\- 4 = Read

\- 2 = Write

\- 1 = Execute



Example:



7 = Read + Write + Execute

5 = Read + Execute



\## sudo

Allows a regular user to execute commands with administrative privileges.



Example:



sudo apt update



\## chown

Changes the ownership of a file.



Example:



chown user file.txt

