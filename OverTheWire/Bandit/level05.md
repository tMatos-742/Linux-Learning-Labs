# Useername

bandit5

# Bandit 5 Password

6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG

# The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable

1033 bytes in size

not executable

So we know that we have the similar senario as the previous level but now we have some specifications. 
This time we now from the beginning that the file is human readable it as 1033 bytes and its is not executable.

After this we go and use the _find_ command again but now we are going to had some arguments to it.
In the _find_ command we have three usable arguments for this situation _-type_,  _-size_ and  _-executable_

<img width="572" height="38" alt="Captura de ecrã 2026-10-11 154437" src="https://github.com/user-attachments/assets/6ab09f55-b365-4437-853c-e864d5f01ae5" />

In each argument we put the information that we have and with it we have our result. Like you see in the above image. 

In size we specified that it is a file with 1033 bytes
In type we say the type of data to be returned, file / directory

In the executable we use _! -executable_ that indicates the file is not executable

After we now what directory and what file to search for we find the password for the next level

<img width="420" height="53" alt="Captura de ecrã 2026-10-11 155027" src="https://github.com/user-attachments/assets/cfdae5a0-21c4-4712-a03a-5533148af2d4" />
