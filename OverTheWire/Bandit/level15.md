# Username 

bandit15

# Password for this level

pbLYuZtTg4MgaqfJx8jbA9gKKGqM68A7

# The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.

Another netcap level for us to continue learning about server connections this one brings us something new since in this one we need to use OpenSSL connection.

Educational moment:

SSL/TLS - This encryption is used to provide communication with a few other networking protocols, most likely HTTPS, which allows for encrypted webpage communication.

This time we will use _openssl_ command to send the password to the port and get the password for the next level. And for that like i said we are going to use _openssl_

<img width="868" height="452" alt="image" src="https://github.com/user-attachments/assets/d2a2c609-76dc-4c01-a98a-76a2cd6b3b4e" />

As you can see there is two ways of doing this. We can openssl to localhost via port 30001 and after you will need to paste the password of the current level so the openssl can give you the next password back.

Or we can use the good old piping that i love and just echo the password in to the openssl and it will retrieve you the password. 
