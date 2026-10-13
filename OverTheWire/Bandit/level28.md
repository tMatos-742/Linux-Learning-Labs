# Username

bandit28

# Bandit 28 Password

y8Yd2ssKcpHpud7UvOSOxwamRMzIGIeQ

# There is a git repository at ssh://bandit28-git@bandit.labs.overthewire.org/home/bandit28-git/repo via the port 2220. The password for the user bandit28-git is the same as for the user bandit28. From your local machine (not the OverTheWire machine!), clone the repository and find the password for the next level. This needs git installed locally on your machine.

Another git repository exercice, remember the git clone that we did in the last level. Let's do it again.

<img width="684" height="31" alt="image" src="https://github.com/user-attachments/assets/577c6369-701e-4922-af2a-41bbc06ec47e" />

After we clone the repository to our local VM we go into the repository folder and see what we need to do this time.

<img width="484" height="328" alt="image" src="https://github.com/user-attachments/assets/4f8057df-e61e-4b97-8200-03960780b9f5" />

OK we have another README file and we see that the password for bandit29 is hidden so we need to find a way to see it before it was hidden. So we need to see the logs for this git repository.

<img width="749" height="327" alt="image" src="https://github.com/user-attachments/assets/0f79f3ae-e6f8-4402-adf4-fb90d14331fe" />

There we go we have 3 changes made to the file. This changes are called commits and each commit as an hash number that we can read.

With git show we can make the command two different ways.

<img width="770" height="314" alt="image" src="https://github.com/user-attachments/assets/61fe9534-949c-402a-b874-ec238bc1153e" />

The first way is what we see in the image above. That indicates what as in the file and what was added. But we can add the name file after the commit hash and we also get the information after the change from the first commit to the second.

<img width="847" height="151" alt="image" src="https://github.com/user-attachments/assets/b994f81f-5326-48de-95b7-15df897b1960" />
