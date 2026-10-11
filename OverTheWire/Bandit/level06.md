# Username

bandit6

# Bandit 6 Password

pXa26xhMWaC2SvDotA4r9EGgZkulOeSBW

# The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7

owned by group bandit6

33 bytes in size

Another level that the _find_ command will help us out. Again we go into our bandit6 via ssh on port 2220.
After we enter the ssh we start to build our find command.

<img width="433" height="18" alt="Captura de ecrã 2026-10-11 160021" src="https://github.com/user-attachments/assets/b356c5ce-dec1-45a7-8d6a-c6f4281804a0" />

 By the image above we can analise the following:

 Command: find
 Arguments:
 -user -> we know that the file is owned by user bandit7
 -group -> we know that the file is owned by the group bandit6
 -size -> we know that the file is only 33 bytes

 BUT!!!! There is a big BUT to this. If you notice after the _find_ command we use the _/_ caracter and right after the _find_ command we need to specifie the location of the file.
 And by using _/_ we saying to the find command to search everyhere in the system and because of that we want to Omit any error message from the output. So we add a final argument.
 
 **2>/dev/null** -  This argument sends everything that we don't find necessary to the "VOID". But i will leave that explanation for the future leves.

 <img width="720" height="36" alt="image" src="https://github.com/user-attachments/assets/9d5bca16-5a02-4373-bc9c-64f7a5142a2e" />

After our command is build we run it and we can see where should we search for our next password.

<img width="467" height="36" alt="image" src="https://github.com/user-attachments/assets/a80d484f-ed30-4293-853d-873ceb878544" />
