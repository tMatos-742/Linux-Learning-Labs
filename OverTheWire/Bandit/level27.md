# Username

bandit27

# Bandit 27 Password

STJLBRRphMxKB392CT4iOr5CbzPU9ER

# There is a git repository at ssh://bandit27-git@bandit.labs.overthewire.org/home/bandit27-git/repo via the port 2220. The password for the user bandit27-git is the same as for the user bandit27. From your local machine (not the OverTheWire machine!), clone the repository and find the password for the next level. This needs git installed locally on your machine.

Ok this means we need to learn a bit about **git** remember to do your research online and you also have _man git_

So we use _git clone_ command to clone the repository that its in bandit27.

<img width="1002" height="367" alt="image" src="https://github.com/user-attachments/assets/c5a691ea-3060-4909-b009-02e8503c38f0" />

Now we need to enter the repository and see what's inside

<img width="577" height="181" alt="image" src="https://github.com/user-attachments/assets/a7571976-f5b8-41db-8b6c-c37923f944d2" />

Inside we find a README file and reading it we find the password for bandit28

Conclusions:

We learn out to clone git repositories from an ssh connection and after that we access the repository and see a README file with the password for level28. 
