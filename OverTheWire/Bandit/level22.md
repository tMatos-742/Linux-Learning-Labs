# Username

bandit22

# Bandit 22 Password

RYVux2rHEm9tiXHmLFzuR7Vhx6AZQMEz

# A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: Looking at shell scripts written by other people is a very useful skill. The script for this level is intentionally made easy to read. If you are having problems understanding what it does, try executing it to see the debug information it prints.

Let's access the cronjob for this level and see what's happening.

<img width="573" height="166" alt="image" src="https://github.com/user-attachments/assets/1e9d87bc-12c4-4af9-94c2-d152d55e1994" />

This script contains a couple of variables called _$myname_ this variable will work with the _whoami_ command to identify the user that is being used in the moment

Since the script identifies what user we are using it copies the password and sends it to a temporary file in the /tmp directory and this file is determined by another variable called _$mytarget_ that we can see that is using _echo_ to send "I am user $myname" piping it to the _md5sum_ command and them to the _cut -d_ command

In the end of the script it is going read the file with the password of bandit23 and send it to the temporary file on the /tmp directory. This temporary file name now as the variable $mytarget is going to be an md5sum hash that is being create in the mytarget variable.

Let'ts let and example: 

<img width="462" height="34" alt="image" src="https://github.com/user-attachments/assets/b32a83a6-5e63-4577-a1fd-1dc12710caca" />

After this we pipe a cut to cut the space and the - in the end of the hash name

Like so:

<img width="602" height="37" alt="image" src="https://github.com/user-attachments/assets/b6bcfa88-d41e-4ef4-82e5-608aa767d27d" />

Know we are going to replicate the command inside bandit22 and by doing this we will find the name of the file that as the bandit23 password.

<img width="581" height="38" alt="image" src="https://github.com/user-attachments/assets/e6274e1a-573b-489b-a1e7-091d53756f29" />

Ok after we replicate the command we find the name for the temporary file now we just need to read the file that contains the password for bandit23

<img width="495" height="35" alt="image" src="https://github.com/user-attachments/assets/e81f0e18-ed7d-4dc0-961b-fe1f9f74f2b9" />

There it is the password for bandit23!!!
