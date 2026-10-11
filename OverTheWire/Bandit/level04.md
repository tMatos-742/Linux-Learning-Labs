# Username 

bandit4

# Bandit 4 Password

xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq

# The password for the next level is stored in the only human-readable file in the inhere directory.

In this statement we already receive an hint on what can be happening in the this level, because in computer files we typically have two types of files, human-readable text and machine readable data
# Let's connect to our bandit4 via ssh and see whats hapenning on this one.

Again we need to _cd_ into the directory **inhere** and we search again for whats inside this directory.

<img width="448" height="271" alt="Captura de ecrã 2026-10-11 150028" src="https://github.com/user-attachments/assets/70591ba1-3c37-496d-8613-a12ee50561bf" />

In this case we have a lot of files and remember we need to find the human readable file and if we _cat_ the file00 we see that this file contains binary inside it.

<img width="443" height="39" alt="Captura de ecrã 2026-10-11 150223" src="https://github.com/user-attachments/assets/e88e4d88-5dc3-4fd5-afad-20cc7037d449" />

What can we do to find the Human Readable file? It would be tedious to go file by file to look for the correct file no? Good thing that there is a way to scan all of them at once

# Solution for this level

For this level we cloud use the command _file_ that returns the type of content is in a file. But remember we would still need to go one by one, so we go and scan all of them by once. 
And for that we use the special character _*_. This is called a wilcard caracter in Linux this is used as a shorthand for "all files".

<img width="274" height="198" alt="Captura de ecrã 2026-10-11 150817" src="https://github.com/user-attachments/assets/692ac647-9148-4a7d-bd76-74e0e40b07ed" />

We can run the commando _file ./*_ like you see in the image above to combine the file command with the _*_ wilcard character to run the command on all the files inside the directory.

After we now what file has the correct content inside we use _cat_ so we can know whats the password for the next level

<img width="348" height="231" alt="Captura de ecrã 2026-10-11 151525" src="https://github.com/user-attachments/assets/d000dea7-05b0-4d65-aac6-fe389541062c" />

Note:

The _Find_ command os used to search for files on the system. It can be used in many different arguments and flags to make your search simpler.
