# Username

bandit32

# Bandit 32 Password

pWuj5jBQ6IgV0NXwiH6g1pXRF8S1YvbT

In this level we are back to connecting to the bandit level through the ssh command like we did many times before...

<img width="401" height="26" alt="image" src="https://github.com/user-attachments/assets/072bead0-690d-42b2-a7e6-ceb320d7274a" />

Let's enter the level password and figure what is going on in this level... So we are welcomed in to a uppercase shell.

<img width="279" height="81" alt="image" src="https://github.com/user-attachments/assets/548c12ed-1663-4395-9c9b-7c91bebc6a27" />

This means that everything we type into this shell will be in UPPERCASE so imagine if we do an _ls -la_ with will automatically be sent to the shell as **LS -LA** and this doesn't exist in linux so we need to figure out a way to overcome this situation.

So we need to use characters that won't be changed into uppercase and that can happen with special symbols and numbers because these don't have an uppercase version of themselfs.

Although in bash we have a special variable called $0 that calls the shell that is available to use. So let's use it.

<img width="532" height="206" alt="image" src="https://github.com/user-attachments/assets/51b9b99d-53d3-44b4-8e86-251a8cb512d3" />

Now we are able to access the bandit32 shell. And since we don't have any indication in the inicial statement lets just go straight to the bandit_pass directory and read the file with bandit33 password.

<img width="587" height="104" alt="image" src="https://github.com/user-attachments/assets/2672b9de-c3d4-4f92-9714-8ae76434a794" />

And like that we have the password for bandit33. Good job!!
