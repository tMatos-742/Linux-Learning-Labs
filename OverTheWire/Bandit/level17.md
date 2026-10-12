# Username 

bandit17

# Bandit 17 Password

SSHKEY that bandit16 gave you last level

<img width="499" height="647" alt="image" src="https://github.com/user-attachments/assets/8fa9e053-446e-4d67-bcb8-cc6c3a3a26df" />

Since the last level gave us an sshkey we need to save it in a file and use that file to access the bandit17 level

<img width="709" height="33" alt="image" src="https://github.com/user-attachments/assets/e1f6f11e-96e8-4df1-849f-b071223b54ea" />

AND DONT FORGET!!! To use the sshkey file that you made you need to make the permissions correct for the file in question.

<img width="408" height="15" alt="image" src="https://github.com/user-attachments/assets/4d52b517-bf4b-477b-87b3-2c97f0832252" />

There are 2 files in the homedirectory: passwords.old and passwords.new
The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

In this level we just need to compare the difference from the passwords.old and passwords.new file and with that we use the command _diff_

<img width="376" height="91" alt="Captura de ecrã 2026-10-12 151102" src="https://github.com/user-attachments/assets/fe71e4d2-2062-4a66-a0b3-f4405229d81a" />

Basically we tell the command to search the difference from old to new file. And as we there was a password that was change from the old to the new file.
