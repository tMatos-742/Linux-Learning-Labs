# Username

bandit14

# Bandit 14 Password

aaWecNkG4FhxJQxz07uiwzVP6bJiYS65

# The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

How can we check if there is a service on this port on the localhost service? We use _nmap_ command.

<img width="1202" height="185" alt="image" src="https://github.com/user-attachments/assets/255692ba-96be-4e69-9e03-c1fa1f090099" />

With the _nmap_ command we can see that there is an unrecognized service running.

In this level we are instructed to send the passowrd of the current level to localhost on port 30000

And with that we introduce the netcap _(nc)_ command that is basically used to connect to services.

There is two ways to do this we can either netcap localhost and after the connect is made we sent him the password or we can go back a couple of levels a use our good friend piping.

<img width="655" height="164" alt="image" src="https://github.com/user-attachments/assets/485fc595-88a0-4c4b-8298-3b604d8e598f" />

In this image as the solution that i explained just now.

