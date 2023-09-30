# CLI (Command Line Interface)

1. \>

```sh
$ ls -lh > file_list.txt
```
- using ">" : create and save the output in a file
- make a file_list.txt about ls -lh 's result

---

2. cat

```sh
$ cat file_list.txt
```
- display the content of a text file

---

3. \>\>

```sh
$ ls -lh >> file_list.txt
```
- if it already exists, append output to an existing file
- if it doesn't exist, create and write to a new file
  - if not use >>, then delete the original file and make a new file

---

4. \<

```sh
$ sort < words.txt > sorted_words.txt
```
- sort the words.txt and make a new file named sorted_words.txt
- put the content of sorting words.txt to sorted_words.txt

---

5. pipelines |
- output of previous command to input of next command

```sh
$ ls -lh | less
```
- if the length of result is too long, use pipeline | and less

```sh
$ ls | wc -l
```
- the number of files in the current directory

---

6. echo (expansion)

```sh
$ echo print out the text
```
- print after echo

```sh
$ echo *
```
- file in present's directory

```sh
$ echo ~
```
- home directory of current user

---

7. backslash

```sh
$ ls -l \
> --reverse \
> --human-readable
```
- ignore line change in command ("enter") to enter a long command in multiple lines

---

8. permission
-  Linux is a multi-user system  
![image](https://github.com/wonhyuna/temp-repo/assets/68580694/9d11e252-b5b8-424c-9674-7ea307209cdd)
- if you don't want to give a permission, just use "-" (ex. -rwxr-xr-x)

---

9. change permission
![image](https://github.com/wonhyuna/temp-repo/assets/68580694/8d5e9192-11f9-4fc9-b65f-137972c7b42d)
- chmod changes permissions
```sh
$ chmod 600 some_file
```
- 6(110) = rw- for owner / 0(000) = --- for group / 0(000) = --- for others

---

10. superuser
- A superuser has all system administation authority
- if you need superuser's privilleges, put "sudo" before the command

```sh
$ sudo some_command
```

```sh
$ sudo -i
```

- exit: to get out of a superuser session

---

11. text editors
![image](https://github.com/wonhyuna/temp-repo/assets/68580694/34fe7a72-5a58-475e-8b39-192f71f7ed49)

---

12. shell script
```sh
$ nano myscript.sh
$ echo "Hello Shell Script!"
$ sh myscript.sh
```
- write and run a shell script

---

13. history
```sh
$ history > history_command.txt
$ cat history
```
- type "history" to see previous command history
- save it to a text file
