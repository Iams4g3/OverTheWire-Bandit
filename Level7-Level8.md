## :triangular_flag_on_post: Level7-Level8
The password for the next level is stored in the file **data.txt** next to the word millionth

> **Solution**
- We log into the game using SSH by typing this command `ssh bandit7@bandit.labs.overthewire.org -p 2220`.
- On the home directory, you will find an ASCII text file called "data.txt". The file has alot of dummy text data
- To extract password from that dummy data, we use `grep` command
  - Type `cat data.txt | grep "millionth"`
    - `|` We use pipe to use the output of one command as an input of another command
    - `grep "millionth"` a command used to extract a specific piece of text/data based on a given pattern (regular expression)

> **Password**
- **dfwvzFQi4mU0wfNbFOe9RoWskMLg7eEc**
