# Username 

bandit20

# Bandit 20 Password

4pIjcunZ0fJ2vmp3IwfG8Vf7VhxD6pOA

# There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. 
It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). 
If the password is correct, it will transmit the password for the next level (bandit21).

This level requires us to run a SUID binary that contacts the localhost port and if that localhost port is outputting the password for bandit20 it will then reveal the next password for bandit21

In this level we need to create a netcat listener since all the ports that are listening in the bandit20 user none of them is broadcasting the password for level bandit21

<img width="717" height="341" alt="image" src="https://github.com/user-attachments/assets/d2b450f0-4955-4acc-b9b9-d2b079f9a692" />

And to create that listener we need to send the password from bandit20 to the port that we want to create.

<img width="524" height="15" alt="image" src="https://github.com/user-attachments/assets/d46ff75b-b993-4f68-814b-b2b673bc643d" />

We use nc -nlvp mode that is no dns lock up, listening, verbose and port number and we especify a port that is not being used and we need to run this as a process.

After we created our port listener we use the SIUD binary file to see if we can have the password for bandit21

<img width="280" height="86" alt="image" src="https://github.com/user-attachments/assets/eb14fa97-8afb-41cc-8ac7-239e1b72d6ae" />

And there we go we got our password
