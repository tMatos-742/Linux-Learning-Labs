# Username 

bandit13

# Bandit 13 Password

qQYQiHOBPR8ZR61qxYqX45quvihF2uzk

# The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user bandit14. For this level, you don’t get the next password, but you get a private SSH key that can be used to log into the next level.
Look at the commands that logged you into previous bandit levels, and find out how to use the key for this level. If you need help with this level: a hint file can be found in the home directory.
Make sure to read the error messages as they are informative.

SSH KEYS! This is a good one....

SSH private keys are an alternative method of login via the ssh program. There is a particular insight that will teach us a new part of linux that is PERMISSIONS.

In order to use an SSH private key we must set a especific type of permissions in to that file. Being that said the ssh key file must not have global or group permissions of any kind.

Since the ssh key is in the ssh bandit13 we need to copy it to our local vm so we can use it for the next ssh connection for bandit14. 

We connect to bandit13 and see in what directory is the file.

<img width="531" height="167" alt="image" src="https://github.com/user-attachments/assets/7b3cc859-3935-402f-89d0-63a875ca7985" />

There you go we found it on the home directory by the name of sshkey.private

Now we need to go back to our local VM and make a copy of this file. In our local VM we are going to use the command _scp_ that is basically the same as _cp_ but for server connections.

<img width="1165" height="260" alt="image" src="https://github.com/user-attachments/assets/ceea3da1-169f-4602-998e-bab4c4be260d" />

After you run this command you will need to insert the bandit13 password and the file will be coppied.

Remember what i said about the file permissions? This is the time that we need to change them.

<img width="526" height="16" alt="image" src="https://github.com/user-attachments/assets/afee5b57-daac-4a2c-a917-88b8a2f3e22c" />

This file need to only have reading and writing permissions for its owner.

<img width="865" height="227" alt="image" src="https://github.com/user-attachments/assets/2b74f85a-570c-4b06-9623-e4a5487bbc7c" />

Let's see what have we made... We change the permissions of the file with the _chmod_ command and set the right permissions so the file can be used.

After that we made the usual ssh command BUT this time we use _-i_ argument so it uses the sshkey.private to access the bandit14 user. 

Since we are inside bandit14 now we just access the /etc/bandit_pass/bandit14 file that was mentioned before.

<img width="396" height="34" alt="image" src="https://github.com/user-attachments/assets/eccb6194-684d-4f6c-aad7-55f06470dbdf" />
