# Username 

bandit12

# Bandit 13 Password 

GROozWPO8QN0mGrjUkID0WCYkZiQxrN

# The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. 
For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. 
Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

There are some things that we can learn for this first statement. Hexdump and compressed files.

So hexdump is usually done in the context of debugging, reverse enginerring and digital forencics. I would recommend to check it out on the web.

Compressed files in computing are often used to reduce size of files obviously. So lets make a directory inside tmp or if you want just go with the statement indication and let the system make one for yourself

<img width="283" height="38" alt="image" src="https://github.com/user-attachments/assets/be34068c-1200-430d-b3c9-cd01364e3600" />

And after it we copy the data.txt file on the home directory to our newly create directory inside tmp.

<img width="580" height="111" alt="image" src="https://github.com/user-attachments/assets/89329881-1175-42ec-8868-5eba0708dc48" />

Ok now that we copied the file and confirmed that it is in our new directory let's start decompressing it. But first we need to reverse the hexdump.

<img width="506" height="130" alt="image" src="https://github.com/user-attachments/assets/aa92ea22-6588-4b42-8977-307e5dba50df" />

So we reversed the hexdump operation with the _-r_ that means reverse and we sent the result to a file called data.

To start decompressing the file we need to know what type of file this file is.

<img width="1167" height="56" alt="image" src="https://github.com/user-attachments/assets/5d6f0afe-5e17-4c14-9505-bfe1cd9f5f65" />

Now that we know it is a gzip compressed file we need to rename our file and give it the gz file extention.

<img width="419" height="108" alt="image" src="https://github.com/user-attachments/assets/21c8dff5-c24e-42f1-bc1c-d6b6e0689c86" />

So we changed the extention of the file and used gunzip do unzip the file and found another data file but now it is another type of file that we need to decompress. And since we know its is a bzip2 file we need to change the file extention again

<img width="1186" height="132" alt="image" src="https://github.com/user-attachments/assets/1ab4adbb-a20f-4b69-8334-5c1744f49c61" />

OK so we changed the file extention again and used bzip2 with -d wich is the decompress argument of the data.bz2 file and after it we found another data file and this time its a gzip file again so we just need to repeat the process.

<img width="426" height="106" alt="image" src="https://github.com/user-attachments/assets/436c30b2-f3cc-4492-a237-dc7970728bd0" />

**Ohhh damm another file inside a file this one is probably going to be long** 

But this time we have a different type of extention. Let's change the file to the correct extention and decompress it!!!

<img width="435" height="57" alt="Captura de ecrã 2026-10-12 113004" src="https://github.com/user-attachments/assets/9e3067ed-a5b6-431c-8496-49de0cb89687" />

Chaging the file to .tar and using tar to decompress it with -xf arguments to extract the file inside data.txt and with that we get a data5.bin file

<img width="486" height="124" alt="image" src="https://github.com/user-attachments/assets/041b2925-e134-4e7d-b121-8a36ecd90bd1" />

Ok let keep repeting the process over and over again. Another tar file we change the extention use the same command to extract the file and we find another file called data6.bin that we see it's bzip2 type of file
Remember what we did a couple of steps back?! Yeah lets run it again.

<img width="1186" height="289" alt="image" src="https://github.com/user-attachments/assets/c04ccd20-df44-41b5-a944-799da2aee292" />

Let's hope this is the last file that we have to decompress

<img width="500" height="109" alt="image" src="https://github.com/user-attachments/assets/a2f17347-20ca-4771-8fc1-f96f0be92a9e" />

YES!!! text file format!!!! We can view its contect now.

<img width="392" height="38" alt="image" src="https://github.com/user-attachments/assets/792bbe29-384c-45bd-8bdb-1f38733800f0" />
