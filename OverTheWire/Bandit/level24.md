# Username

bandit24

# Bandit 24 Password 

hVQMk3lJNsmQ7VF3ubyrNNBom7BOgVXv

# A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing. You do not need to create new connections each tim

In this level we need to create a bash command that will try the 10000 combinations at once so we can have the password for bandit25.

In this one we need to create a loop. And we want that loop to go in between 0 and 10000. But at the same time we need to send the password, because the bandit25 password will only be retrieve if we send the bandit24 password at the same time we try to figure out the 4 digit code.

With that said we are going to use piping and other commands.

<img width="1206" height="197" alt="image" src="https://github.com/user-attachments/assets/784d3dcd-9f20-47b2-baba-6f50e819be91" />

I think we can do better than this let's use our old friend _grep_ to filter want we don't want to see.

<img width="1202" height="130" alt="image" src="https://github.com/user-attachments/assets/37bd2807-34b6-4757-80fc-0fd46ef91d1b" />

There we go with grep we removed every result that started with Wrong! because that was basically the message that appear every time the pin code was wrong. Basically instead of having 9999 messages saying "Wrong Password" we just got the password for bandit25. 
