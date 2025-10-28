## :triangular_flag_on_post: Level1-Level2
The password for the next level is stored in a file called - located in the home directory
> **Given Information**
  1. username: bandit1
  2. password: ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If
  3. ssh port: 2220
  4. Host: bandit.labs.overthewire.org

> **Solution**
- We log into the game using SSH by typing this command `ssh bandit1@bandit.labs.overthewire.org -p 2220`
- Take a look at the content of the current working directory/home directory using `ls`
- Like the information in our challenge description, we found a file named **-**. To open this file, we open it by calling it based on its location on the file system thus `cat ./-`

> **Password**
- **ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If**
