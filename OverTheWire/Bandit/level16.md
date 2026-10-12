# Username 

bandit16

# Bandit 16 Password

kS0Hf0u5HiXFwKMKFqXvOdOTNGGa0X8V

# The credentials for the next level can be retrieved by submitting the password of the current level to a port on localhost in the range 31000 to 32000. 
First find out which of these ports have a server listening on them. Then find out which of those speak SSL/TLS and which don’t.
There is only 1 server that will give the next credentials, the others will simply send back to you whatever you send to it.

Let's do this by the steps that we have the incial statement. First of all we are going to search in a specific range of ports that are serving SSL to localhost and after that send the password to the port.

<img width="670" height="330" alt="image" src="https://github.com/user-attachments/assets/ae159afb-8e37-4b67-b4f4-74a765b65667" />

With this command we can see a couple of ports that are open in the specified range that we stated. We just need to wait for the end map to finish is search and tell us which port is running SSL

<img width="376" height="105" alt="image" src="https://github.com/user-attachments/assets/a9ff5e2f-fd8c-4342-a3e2-7aef5c8da105" />

In this image we can see that port 31518 abd 31790 are using SSL services. Although 31518 is also using echo services this means that the port we are using to send our password is 31790.

<img width="873" height="356" alt="image" src="https://github.com/user-attachments/assets/ebba552c-d960-4490-a81d-7b1313bb43b1" />

We did it!!! As you can see we got the correct way of doing it, but we got a sshkey but this time we cannot copy a file to our local VM and use it for the next ssh connection so we are going to need to copy the full sshkey.
