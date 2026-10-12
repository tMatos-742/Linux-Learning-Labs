# Username 

bandit11

# Bandit 11 Password

pYfOY6HwUsDj5rL9UvyhU7MCmv8vN5Ro

# The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

Rotating letters by 13 positions is this somekind of sorcery? Nahhh just another encryption method called ROT13 let's learn a bit about it, don't forget to search in the Web about and try to get more information about it.

ROT13 is a simple substitution cipher where the encryption method shifts each plaintext letter 13 positions in the alphabet to from the ciphertext.

Example:

<img width="475" height="232" alt="image" src="https://github.com/user-attachments/assets/7efbc492-9450-45e5-8c7f-d3c23ad3e29f" />


Encryption example:

<img width="373" height="208" alt="image" src="https://github.com/user-attachments/assets/61516521-0201-4c2b-b92a-53c451054f3e" />

Basically like we see in the image above after using the cipher to encrypt the plaintext the result will be 13 positions ahead of the original one.

Now that we learn a bit about another encryption method lets build our code so we can get our objective. But we need to introduce a new command. _tr_

_tr_ is used to transform characters in to other characters and it can be used to simulate ROT13 decryption. Ok now lets build our command.

<img width="496" height="38" alt="image" src="https://github.com/user-attachments/assets/0d779f9c-666c-4417-af28-f68072d63d5a" />

So if you search for ROT13 on the web expecially on the wiki you will get a create explanation of what happened and basically we mapped upper and lower case A-Za-z to N-ZA-Mn-za
Meaning that you want to rotate the characters positions by 13. 
