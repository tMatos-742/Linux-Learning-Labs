# Username 

bandit29

# Bandit 29 Password

Em7eGtqaMySwNFjCpWzzHhLhospOcdt0

# There is a git repository at ssh://bandit29-git@bandit.labs.overthewire.org/home/bandit29-git/repo via the port 2220. The password for the user bandit29-git is the same as for the user bandit29.

We copy the repository and after going into to the repository directory we see another README file and we read it.

<img width="480" height="255" alt="image" src="https://github.com/user-attachments/assets/3138344e-eae0-47b8-950e-97c852e585e3" />

Another file with no password. Let's check the log again.

<img width="766" height="154" alt="image" src="https://github.com/user-attachments/assets/6f878e37-449a-44fb-aec3-98910c4bec8c" />

Nothing again on the first commit change for the file. So after this we need to check if there are branches inside the repository maybe the file with the password is somewhere else.

<img width="407" height="148" alt="image" src="https://github.com/user-attachments/assets/f4a69545-de66-4dcb-bd0b-97792b2da922" />

There it is we have more branches probably there is more files inside each branch and one of them can have our password.

Let's go into the _dev_ branch this might mean that its the branch that onyly dev's use and our password can be there

<img width="415" height="53" alt="image" src="https://github.com/user-attachments/assets/4c568cac-13e0-4913-9a54-68d3a8e7c0fd" />

We can confirm that we are in the correct branch by using another command

<img width="360" height="97" alt="image" src="https://github.com/user-attachments/assets/0743bbf8-dc3b-4527-b02d-cf29ec558798" />

There you see that the branch that you is with green letters. Let's see what in this repository.

<img width="476" height="144" alt="image" src="https://github.com/user-attachments/assets/9aa252ea-7e5a-41bc-8ee5-c7b51ac2a8d7" />

Another README file....

WAIT!!!

<img width="408" height="155" alt="image" src="https://github.com/user-attachments/assets/592ea323-22f6-4c45-b7a4-535ade1503bf" />

THATS OUR PASSWORD!!!!


