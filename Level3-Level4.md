## :triangular_flag_on_post: Level3-Level4
The password for the next level is stored in a hidden file in the inhere directory.
> **Given Information**
  1. username: bandit3
  2. password from level 3: MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx 
  3. ssh port: 2220
  4. Host: bandit.labs.overthewire.org

> **Solution**
- We log into the game using SSH by typing this command `ssh bandit3@bandit.labs.overthewire.org -p 2220`.
- We navigate inside the **inhere** directory by typing `cd inhere`
- Since the file containing the password is hidden, we need to list all the files found within this directory even the hidden ones. To do that we type `ls -al`
- The output of the listing command shows there is a hidden file called **"..Hiding-From-You"**
- To open this file, we type `cat ..Hiding-From-You`

> **Password**
- **2WmrDFRmJIq3IPxneAaMGhap0pFhF3NJ**
