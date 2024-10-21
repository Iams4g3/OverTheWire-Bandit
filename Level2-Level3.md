## :triangular_flag_on_post: Level2-Level3
The password for the next level is stored in a file called spaces in this filename located in the home directory
> **Given Information**
  1. username: bandit2
  2. password from level 2: 263JGJPfgU6LtdEvgfWU1XP5yac29mFx 
  3. ssh port: 2220
  4. Host: bandit.labs.overthewire.org

> **Solution**
- We log into the game using SSH by typing this command `ssh bandit2@bandit.labs.overthewire.org -p 2220`.
- After login we take a look at the content of our working directory/home directory. We find a file name with spaces
- Normally, we could just open a file by typing a `cd filename`, but however, the file name is spaced so it won't play very well with the terminal.
- In that case we could enclose our file name with quotation marks or hitting `TAB` the moment we start writting the initials of our file name
- So, to open a file we type `cat "spaces in this filename"`

> **Password**
- **MNk8KNH3Usiio41PRUEoDFPqfxLPlSmx**
