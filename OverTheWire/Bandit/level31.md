# Username 

bandit31

# Bandit 31 Password

82NkymblpGBYmIXG6ZQ8YldBYstHpfUf

# There is a git repository at ssh://bandit31-git@bandit.labs.overthewire.org/home/bandit31-git/repo via the port 2220. The password for the user bandit31-git is the same as for the user bandit31.

Ok let's clone the repository and get in to it. 

<img width="518" height="294" alt="Captura de ecrã 2026-10-13 172047" src="https://github.com/user-attachments/assets/2aca8965-7d3d-450e-9979-93d6a0b8bd2f" />

We open the README file and it says that we need to make a file with a specific content in it and put in the master branch of the git repository.

First things first let's make sure we are in the correct branch and after that make the file.

<img width="600" height="235" alt="Captura de ecrã 2026-10-13 172844" src="https://github.com/user-attachments/assets/06cbd63d-6818-42d2-9f67-cb565cd04ccc" />

File created, branch confirmed now lets send the file to the repository. Wait something i didn't saw before we have a file called .gitignore this is probably a script that tell to ignore something that we do let's check it.

<img width="466" height="37" alt="image" src="https://github.com/user-attachments/assets/66e5e99b-d978-46a0-a574-11a8d48b99b1" />

There we go good thing that we checked this file...... This is basically telling git to ignore every file that as the extension .txt. 

So that means we need to force our way into send our file to the repository.

And for that we use **git add -f** the-**f** argument its used to force our way into sending our file to the repository.

<img width="173" height="35" alt="image" src="https://github.com/user-attachments/assets/e6b9dd94-d451-44cd-aa6b-73a5908507b0" />

Ok we add the file to the repository but we need to check if it went trought first, but lets just add a commit to it so we can identify what was done to it.

<img width="235" height="33" alt="image" src="https://github.com/user-attachments/assets/3947bb6b-e55c-4250-b039-13c2fff7afa4" />

Commit done lets check its status and send it to the repository

<img width="432" height="82" alt="image" src="https://github.com/user-attachments/assets/686cb96b-4bbb-4214-938c-d9de27f06849" />

We can see that the status tells us that our branch as 1 commit and that we need to push it to the repository.

<img width="626" height="673" alt="image" src="https://github.com/user-attachments/assets/5c76a2c3-180d-4e63-aad5-e004dcc5be3a" />

We push the file to the repository and it will ask us for the bandit31 password. After we give the password it will retrieve the bandit32 password back.

CURIOUS NOTE:

Did you notice at the end of the output is said [remote rejected] master -> master (pre-receive hook declined) this can be called normal. The server probably has an hook script that validates the content of our file gives us the password confirming that our file is correct but refuses the push so it doesn't get full with files that don't matter that the repository can consider to be garbage. And since we have our password we can just ignore the error.





