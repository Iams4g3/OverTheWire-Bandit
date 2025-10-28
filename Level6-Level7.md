## :triangular_flag_on_post: Level6-Level7
The password for the next level is stored somewhere on the server and has all of the following properties:
1. Owned by user bandit7
2. Owned by group bandit6
3. 33 bytes in size

> **Solution**
- We log into the game using SSH by typing this command `ssh bandit6@bandit.labs.overthewire.org -p 2220`.
- Since the file is somewhere on this linux server, the best place to begin our search is on the root directory of the server which is `/`
- Using the knowledge we got from the [previous](https://github.com/Iams4g3/OverTheWire-Bandit/blob/main/Level5-Level6.md) challenge, we run `find / -group bandit6 -user bandit7 -size 33c -type f` to get the file holding the password
- However, the output generated to the stdout contains error messages warning us the permission to search/view/access certain location is denied.

![Lvl6-Lvl7](https://github.com/Iams4g3/OverTheWire-Bandit/blob/main/Resources/Lvl7-Screenshot.png)
  - But if you scroll slowly through the output containing error messages, you will find the location of a password file hidden in plain site.
  - The best idea here is to filter/separate the error messages output from the file location which is the real output
- To achieve that, we write `find / -group bandit6 -user bandit7 -type f -size 33c 2> /dev/null` to get the location of a file containing the flag
  - `2>/ dev/null` Means we are redirecting stderr (printer errors) to the location `/dev/null`
  - The `/dev/null` is a location considered as a blackhole. Meaning it disregards anything written on it. So, by writting the errors to this location we are basically disposing the errors we dont need to view
- Now since we have the location of the file that we need, type `cat /var/lib/dpkg/info/bandit7.password` 



> **Password**
- **morbNTDkSW6jIlUc0ymOdMaLnOlFVAaj**
