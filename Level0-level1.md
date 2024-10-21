## :triangular_flag_on_post: Level0-Level1
The password for the next level is stored in a file called readme located in the home directory.
> **Given Information**
  1. username: bandit0
  2. password: bandit0
  3. ssh port: 2220
  4. Host: bandit.labs.overthewire.org

> **Solution**
- We log into the game using SSH by typing this command `ssh bandit0@bandit.labs.overthewire.org -p 2220`. Notice that the password used for the [**Level0**](https://github.com/Iams4g3/OverTheWire-Bandit/blob/a213f31b3729732fbfa7a1f488deefc6ea1f5bf4/Level0.md) is the same as the password that is being used to go up a level, thus from Level0 to Level1
- After login we take a look at the content of our home directory/current working directory `bandit0@bandit:~$ ls`
- Just like our challenge description said, we found a file called ***readme***. So what we do now is to open the file to see the content which is the password.
- So, we type `cat readme` and press enter

> **Password**
- **ZjLjTmM6FvvyRnrb2rfNWOZOTa6ip5If**
