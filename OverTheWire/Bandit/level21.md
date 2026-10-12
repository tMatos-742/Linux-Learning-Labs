# Username 

bandit21

# Bandit 21 Password

# There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. 
It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). 
If the password is correct, it will transmit the password for the next level (bandit21).

In this level we are required to inspect cronjobs, cronjobs are commands that are running at regular intervals, the time-based job scheduler. There's a cronjob setup for the bandit22 user.

<img width="504" height="323" alt="image" src="https://github.com/user-attachments/assets/9a31e574-90f9-49b0-bacf-112017f36a3f" />

Before taking any conclucions we need to study cronjobs. Search the internet use AI Agent do your thing.

So now that we got more information on cronjobs we can see that this cronjob is running every minute. We need to see whats happening in the file that is listed in the cronjob.

<img width="496" height="94" alt="image" src="https://github.com/user-attachments/assets/6b8a9f5d-d667-43f2-9fa3-e68e809728ec" />

We know that this is a script file because we can see the prefixe /bin/bash 

Also the script tells us that the permissions of the file in /tmp directory are changed making it readable by all users, it then copies the password for bandit 22 user into it.

In conclusion we need to read the file in the /tmp directory to see the bandit22 password

<img width="449" height="35" alt="image" src="https://github.com/user-attachments/assets/4ba1b32a-8f38-424b-8727-c054550a4f77" />
