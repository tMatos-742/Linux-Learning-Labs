# Username 

bandit8

# Bandit 8 Password

VR1ljMayciFxbnUokuQmJFw6QC9VKtub

# The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

Let's get a good interpertacion of this statement. Basically we need to find in the data.txt file a line of text that occurs only once. 

This means that we are introducing in this level we are going to introduce a couple of commands that are going to help us output only what we really need and that is bandit9 password.  

We start with _sort_ this command takes all the lines contained in a given file and returns them in alphabetical / numerical order.

**You can try doing it in this level, BUT!! you have been warned I WOULDN'T DO IT. BUT YOU DO YOU.** -> "sort data.txt"

The second command will be uniq this takes all the lines in a file and removes any lines with identical contents. This commando is every useful for removing consecutive blank lines in the file in use. -> "uniq data.txt"

Last but not least and maybe the important part of this level is the command Piping. In linux the command piping is the process of passing the output of one command into the input of the second command

Where is an example:

<img width="645" height="81" alt="image" src="https://github.com/user-attachments/assets/9f1d6fdc-2a96-4da5-bd22-6d8caa89b004" />

This is a very useful feature, because it allows commands to be chained together.

# Solution for this level

<img width="340" height="25" alt="Captura de ecrã 2026-10-11 170045" src="https://github.com/user-attachments/assets/46318d5c-8c01-4cdf-95ea-f1c48fbe624a" />

This will output a lot of content but since we used the flag _-c_ in the _uniq_ command this flag will count how many time does a line repeat itself.
In the statement we can see that we need to look for the line that occurs only once

<img width="317" height="57" alt="bandit8" src="https://github.com/user-attachments/assets/42f39377-9e0a-4d88-a136-07b431cf0158" />



