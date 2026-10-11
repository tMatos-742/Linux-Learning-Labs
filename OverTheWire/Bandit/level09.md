# Username

bandit9

# Bandit 9 Password

EjmOSvuAu7sGAHqHVcBDPirRe9T03kxl

# The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

So in this statement we can see that strings could be in use. Let's get into bandit9 like we always do and see whats up.

After we accessed bandit9 via ssh we do the normal command _ls -la_ to see what in the home directory of this level.

<img width="575" height="175" alt="image" src="https://github.com/user-attachments/assets/c9a43991-53c4-460f-ba70-4ea012756615" />

We identify a file called **data.txt** and with that we do the normal _cat_ command. WHAT WAS THAT SO MANY STUFF!!! 

Wait that is just binary data. Files that contain binary data will output random caracters and output gibberish.

Let's go back to the strings maybe thats the way. Strings is a command used to return human-readeable text from files. 
It is often used to find text inside of files that also contain text and binary data.

With this said lets use the command!!!

# Solution for this level

<img width="314" height="22" alt="image" src="https://github.com/user-attachments/assets/ed70f8f5-8833-4a76-a3c6-04264447003e" />

Well that's another file full of information. WAIT!!! Didn't we just learn _grep_ in the last level? And the inicial statement says that the password is next to severeal '='

Lets build another command this time to get the password for the next level.


<img width="506" height="107" alt="image" src="https://github.com/user-attachments/assets/95ea0f5f-e715-4ae2-8e88-69121eefdfe5" />

There you go sucess!!!
