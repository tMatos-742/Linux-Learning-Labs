#Level 0
# The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. 
The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.

# Username
bandit0

# Password
#bandit0

# Solution for this level

ssh bandit0@bandit.labs.overthewire.org -p 2220

# After connection established with bandit0 we move to level0 -> level1
#The password for the next level is stored in a file called readme located in the home directory. 
Use this password to log into bandit1 using SSH. Whenever you find a password for a level, use SSH (on port 2220) to log into that level and continue the game.

# Solution for this Level

ls
cat readme
