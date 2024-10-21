## :triangular_flag_on_post: Level4-Level5
The password for the next level is stored in the only human-readable file in the inhere directory
> **Given Information**
  1. username: bandit4
  2. password from level 4: 2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ 
  3. ssh port: 2220
  4. Host: bandit.labs.overthewire.org

> **Solution**
- We log into the game using SSH by typing this command `ssh bandit4@bandit.labs.overthewire.org -p 2220`.
- We navigate inside the **inhere** directory by typing `cd inhere`
- Inside we find couple of files from which only one is human-readable and is the one with the password.
- Now, we check the file type of all the files in this directory to determine which is human-readable. We achieve this by typing command `file ./*`
- The file that contains the password is an "ASCII text" file as seen below

![Level 5 writeup](https://github.com/Iams4g3/OverTheWire-Bandit/blob/c034952bd2e5a7db051333e83096030da5823ed1/Resources/lvl5-Screenshot.png)

- Opening an ASCII file to view the password, we type the following command `cat ./-file07`

> **Password**
- **4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw**
