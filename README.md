# Lab02
Second Lab Assignment
## Lab 02

- Name: Keonje Paige
- Email paige.34@wright.edu

## Part 1 Answers

Command to SSH to AWS instance:
```
ssh -i "C:\Users\Je\Downloads\labsuser-25.pem.txt" ubuntu@52.45.65.114
```

## Part 2 Answers

1. `chmod u+r bubbles.txt`
    - Means:
It will give the users the access to read the text file
2. `chmod u=rw,g-w,o-x banana.cabana`
    - Means:
u=rw is the change of permissions that users will not be able to execute, but read and write.
g-w removes the group's ability to write in the file
o-x removes the other's ability to execute in the file
3. `chmod a=w snow.md`
    - Means:
This command removes all the permissions of all the groups except for the writing permissions
4. `chmod 751 program`
    - Means:
This command will refer to the three seperate permissions (owner,group,and others) have access of permissions.
Owners will have all three of the permissions, groups would have access to only reading and excuting, and others
will only be able to excute.
5. `chmod -R ug+w share`
    - Means:                              
    This command will recursively add the writing permission for both the owner and the group
## Part 3 Answers

1. Command to create new user:
The sudo useradd -m bob was what helped me addde user "bob" into the terminal
2. Path to user's home directory:
echo $HOME was the command that shows the path of the user's home directory, /home/ubuntu
3. Evaluate if `ubuntu` can add files to user's home directory:
Ubuntu can add files since it has the writing permission
4. Command to switch to user:
5. Command(s) to go to user's home directory:
6. Evaluate if user can add files to user's home directory:
I was able to add a file into the user's directory under bob by making a testfile by using the following command,
touch /home/bob/testfile
7. Command to switch to `ubuntu`:
The command used to switch back to ubuntu was the same su command just with a different destination,
su ubuntu
8. Command to return to `ubuntu` home directory:
To return to the ubuntu home directory, it takes the usuage of the cd /home/ubuntu command, or simply cd
## Part 4 Answers

For each, write the command used or answer the question posed.

1. Command to create group named `crew`:
The command that was used to help me add the group "crew" was the sudo groupadd crew command
2. Command(s) to add `ubuntu` & user to group `crew`:
sudo usermod --append --groups crew ubuntu
sudo usermod -aG crew bob
The two commands above were different wayd to add users to a crtain group
3. Command to modify `share` to have group ownership of `crew`:
sudo chown :crew share
This was the command used to help give "share" ownership of the group "crew"
4. Command to switch to user:
su - bob
Used to switch to the user bob once again
5. Command to add file to `share`:
I was able to add a testfile in the share directory by using the touch command
6. Evaluate why these This command will recursively add the writing permission for both the owner and the group
## Part 3 Answers

1. Command to create new user:
The sudo useradd -m bob was what helped me addde user "bob" into the terminal
2. Path to user's home directory:
echo $HOME was the command that shows the path of the user's home directory, /home/ubuntu
3. Evaluate if `ubuntu` can add files to user's home directory:
Ubuntu can add files since it has the writing permission
4. Command to switch to user:
5. Command(s) to go to user's home directory:
6. Evaluate if user can add files to user's home directory:
I was able to add a file into the user's directory under bob by making a testfile by using the following command,
touch /home/bob/testfile
7. Command to switch to `ubuntu`:
The command used to switch back to ubuntu was the same su command just with a different destination,
su ubuntu
8. Command to return to `ubuntu` home directory:
To return to the ubuntu home directory, it takes the usuage of the cd /home/ubuntu command, or simply cd
## Part 4 Answers

For each, write the command used or answer the question posed.

1. Command to create group named `crew`:
The command that was used to help me add the group "crew" was the sudo groupadd crew command
2. Command(s) to add `ubuntu` & user to group `crew`:
sudo usermod --append --groups crew ubuntu
sudo usermod -aG crew bob
The two commands above were different wayd to add users to a crtain group
3. Command to modify `share` to have group ownership of `crew`:
sudo chown :crew share
This was the command used to help give "share" ownership of the group "crew"steps allowed the above action:
The groupadd command was what help me created the "crew" group,
The commands earlier help me add users to the group.

## Part 5 Answers

For each, write the command used or answer the question posed.

1. Command to create file using `sudo`:
The command used to perform this task is sudo touch sudotestfile.md
2. Evaluate (in plain text) the permission of the file:
The file will only have the owner be able to read and write, Group will only read, and Others will also only read
3. Provide a method to edit the file without modifying permissions:
 sudo nano sudotestfile.md
This command that helps me enter the file through nano is one method without changing permissions
4. Command(s) to modify permissions:
sudo chmod 777 sudotestfile.md
sudo chmod g-w sudotestfile.md
sudo chmod u-w sudotestfile.md
## Citations

To add citations, provide the site and a summary of what it assisted you with.  If generative AI was used, include which generative AI system was used and whatThis command will recursively add the writing permission for both the owner and the group
## Part 3 Answers

1. Command to create new user:
The sudo useradd -m bob was what helped me addde user "bob" into the terminal
2. Path to user's home directory:
2. Path to user's home directory:
echo $HOME was the command that shows the path of the user's home directory, /home/ubuntu
3. Evaluate if `ubuntu` can add files to user's home directory:
Ubuntu can add files since it has the writing permission
4. Command to switch to user:
5. Command(s) to go to user's home directory:
6. Evaluate if user can add files to user's home directory:
I was able to add a file into the user's directory under bob by making a testfile by using the following command,
touch /home/bob/testfile
7. Command to switch to `ubuntu`:
The command used to switch back to ubuntu was the same su command just with a different destination,
su ubuntu
8. Command to return to `ubuntu` home directory:
To return to the ubuntu home directory, it takes the usuage of the cd /home/ubuntu command, or simply cd
## Part 4 Answers

For each, write the command used or answer the question posed.

1. Command to create group named `crew`:
The command that was used to help me add the group "crew" was the sudo groupadd crew command
2. Command(s) to add `ubuntu` & user to group `crew`:
sudo usermod --append --groups crew ubuntu
sudo usermod -aG crew bob
The two commands above were different wayd to add users to a crtain group
3. Command to modify `share` to have group ownership of `crew`:
sudo chown :crew share
This was the command used to help give "share" ownership of the group "crew" prompt(s) you fed it.
https://phoenixnap.com/kb/how-to-create-sudo-user-on-ubuntu
This helped me see what was needed to add users on sudo
https://www.redhat.com/en/blog/linux-groups#:~:text=January%2012%2C%202023Shiwani%20Biradar,the%20/etc/group%20file.
This source was what help assited me on using groupadd commands 
Google AI Overview
This helped by showing exmaple commands of the tasks I described to it from the layout. Such as how to use the permission commands and the three group meanings.