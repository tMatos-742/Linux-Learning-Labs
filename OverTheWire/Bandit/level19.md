# Username

bandit19

# Bandit 19 Password

KpsOfPkcP7u1FlIExm20Ejyt6dw8dxZI

# To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. 
The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

We connect to bandit19 and we find some new stuff....

<img width="486" height="178" alt="image" src="https://github.com/user-attachments/assets/b212569f-70db-47ad-9436-12c614962303" />

In the first statement there is some talk about binary, and this bandit20-do file goes directly to it. And we can see it on the file permissions when we see the "s" value next to the owner permissions.

<img width="447" height="19" alt="image" src="https://github.com/user-attachments/assets/54172a5b-1ed7-4cef-962b-b1ca49a8d640" />

This file is a SUID binary that runs as the user bandit20 and this file will always run in context of its file owner permissions. This meaning we are basically bandit20 when we are using this file.

OK so after this we can try and see if we have access to the /etc/bandit_pass folder.

<img width="456" height="69" alt="image" src="https://github.com/user-attachments/assets/c92aceca-80ee-4b91-8122-49cd4dbba839" />

Quick explanation so we tried to access the folder that contained the password as bandit19 and we got "Permission denied". 
And as you can see by running the bandit20-do its like you became the user bandit20 and know since you act like bandit20 you can access the file with the password that we need.
