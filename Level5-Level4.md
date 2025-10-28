## :triangular_flag_on_post: Level5-Level6
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:
1. human-readable
2. 1033 bytes in size
3. not executable   

> **Solution**
- We log into the game using SSH by typing this command `ssh bandit5@bandit.labs.overthewire.org -p 2220`.
- We navigate inside the **inhere** directory by typing `cd inhere`
- Upon navigating inside, you'll quickly realize that it is a never ending location where different files are being stored. From binary files to normal text files with multiple passwords that don't work (just my assumptions)
- Practically, the only way to get the right file quickly is to run the run command with the right conditions (Properties) so as to get the right file that we need
- We run `find ./ !(-executable) -size 1033c`
  - Use `find` a command used to find a certain file or directory based on a specified criteria
  - `./` specifies where in the file system do you want `find` to begin its search. In my case I navigated inside the inhere directory before running the `find` command on the same directory
  - `!(-executable)` since the criteria required a file to be a non-executable file, I used a `!` operator to negate the condition.
  - Lastly, `size 1033c` the size of a file is in bytes, so specifying the size of a file helped isolating the rest of normal files (Read man page)


> **Password**
- **HWasnPhtq9AVKe0dmk45nxy20cvUa6EG**
