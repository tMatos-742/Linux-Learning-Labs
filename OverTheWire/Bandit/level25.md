# Username

bandit25

# Bandit 25 Password

SoHfqMOEqIX2IYKVciZxvgpR9a2Djx4P

# Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.


<img width="634" height="288" alt="image" src="https://github.com/user-attachments/assets/f29b2ade-3bfb-41c4-a177-54d188f6d015" />

Look another sshkey remember what we did in the past? To copy the file to our local vm and then use it to access the next level? That's what we need to do again. But this time something's different, oh the permissions are already correct we don't need to do nothing against it. NICE!

<img width="1199" height="343" alt="image" src="https://github.com/user-attachments/assets/e5408e7c-d861-4dba-9195-ed914d897a9a" />

That's it we have the sshkey in our local VM now. Now let's connect to level26 and get the password for it.

<img width="1166" height="39" alt="image" src="https://github.com/user-attachments/assets/5fd3f33b-d757-4e67-b5d9-6ed34ba99bed" />

Ohh wait remember the inicial statement bandit26 is not /bin/bash some how we need to try and change that.

Let's go back to bandit25 and check what is the shell of bandit26

<img width="646" height="44" alt="image" src="https://github.com/user-attachments/assets/2817069d-35f5-41f9-83b2-7222cfc5e8de" />

Let's connect again to our ssh connection but we still get disconnected from the ssh connection.... Oh wait it must be because the shell is showtext and not bin/bash

This must be strange but we need to make our windows smaller. Let me explain the way to solve this part is to make the text big enough or small enough to force the _--More--_ to activate and don't show all the text

We can either zoom in on the text or make the text smaller by using the command stty and termining how many rows we want to see for this we use

<img width="467" height="28" alt="Captura de ecrã 2026-10-13 150841" src="https://github.com/user-attachments/assets/65f9807f-34a9-457a-a00e-58aae95e588f" />

And now we do the ssh connection again

<img width="399" height="131" alt="image" src="https://github.com/user-attachments/assets/ccebb94a-1159-4421-b477-0567f2fc6877" />

That is what we want YES we did it!!

Ok now!! Did you know its possible to that we can activate the vim or vi command when we are in a --More-- situation by hitting the letter **v** on your keyboard

If you didn't know you now. Let's do it.

<img width="393" height="114" alt="image" src="https://github.com/user-attachments/assets/a123bc74-4e93-42bc-9a4b-eeb90aea9240" />

WE IN!!!! NICE!!! 

Ok now remember bandit26 wasnt a /bin/bash shell we need to change that ok. Let's get to work.

<img width="386" height="112" alt="image" src="https://github.com/user-attachments/assets/a048a332-e81f-4c06-82a2-14126a19be09" />

We set the shell to /bin/bash and now we try to access it.

<img width="379" height="117" alt="image" src="https://github.com/user-attachments/assets/cbffcf27-7cd9-4dc4-8cc8-064e18dc8234" />

DONE! We are inside bandit26 let's get our password.

<img width="450" height="44" alt="image" src="https://github.com/user-attachments/assets/f169c57e-d358-4e78-8c91-957c4d0358ab" />

That was a difficult one. 

Conclusion: 

So basically we got the sshkey from bandit25 copied to our local VM machine used another ssh connection to enter bandit26 we couldn't because some one change the configuration an also changed the shell format of bandit26 and we confirmed that its was changed to showtext.
After this we made the terminal only show 5 rows and we activated the _--More--_ option and with that we could activate the vi command and change the shell type of bandit26. After we sucessfully change the shell type we reed the bandit26 password file located on /etc/bandit_pass.


