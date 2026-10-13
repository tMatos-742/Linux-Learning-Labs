# Username

Bandit23

# Bandit 23 Password 

gKXDTAXnIz3OBxiPjRZ2uqutUlPZrBsw

# A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: This level requires you to create your own first shell-script. 

<img width="583" height="388" alt="image" src="https://github.com/user-attachments/assets/2e8a7881-1f5f-4be3-9897-32bbba731f54" />

So this is a lot complex compared to the last level. Let's get and interpertacion and read the script.

Fist of we see the same variable myname from the last level doing exactly the same. After it moves into /var/spool/$myname/foo and _echo_ the message "Executing and deleting all scripts" in the same directory that he just moved into.

Essencially that's it the for loop that we see below its basically deleting every script inside that folder every 60 seconds.

So we can write our own script in that directory and have bandit24 execute our script when the cronjob happens and then retrieve the password that we are going to send to a file inside /tmp directory

Now let create our file

<img width="453" height="23" alt="image" src="https://github.com/user-attachments/assets/94d5f150-888d-48c5-a91b-cb22af38979f" />

We need to create the file in the same directory as the script is being executed.

<img width="790" height="86" alt="image" src="https://github.com/user-attachments/assets/5d58dac5-f73f-4667-ac57-9c550fe22f3d" />

So our script is going to access the bandit24 password and send it to the file inside the /tmp directory like we said before. But we need to give execute permissions to our file but since the file is created we only have one minute to do it until it is deleted.

We can either make the file, edit it and change the permissions or we can do all that in one command. I find it better because we can do it one just one command instead of do it in various steps and if you take your time to do it the file can be already deleted.

<img width="1215" height="87" alt="image" src="https://github.com/user-attachments/assets/fc70e56b-5d4c-4714-8dff-8363fbc674bb" />

So we are use echo to create our script and we say in it that we want to read the password for bandit24 and send it to the tmp directory file name bandit24password.txt. After that we change the permissions for our new folder so the inicial script can execute our file. 

And with that we have have the password for bandit24.


