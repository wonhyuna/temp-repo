# Git
- For using a version control system for software development and other documentation works

1. Changes vs Snapshots(Git)
![image](https://github.com/wonhyuna/temp-repo/assets/68580694/799a452b-de46-4eed-8b15-c4fcac2938c6)

---

2. Local, Centralized, and Distributed Version Control
- Local Computer & Server Computer
- NowDays, using a distributed version control
![image](https://github.com/wonhyuna/temp-repo/assets/68580694/458fbd37-c618-4044-920d-4e9319912c77)

---

3. Three Stages in Git
- Modified, Staged, Committed
![image](https://github.com/wonhyuna/temp-repo/assets/68580694/a7d23f49-ab9a-4c23-b411-e7245b7e8506)

---

## Code

1. Checking git install state
   - Check pre-installed version, if not install git
```sh
$ git --version
```

2. Git config [System -> Global -> Local]  
  a) System Level: --system option (Affects all uses and repositories on the system (administrative))
    -> file: /etc/gitconfig  
  b) Global (user) Level: --global option (Affects all repositories of a current user) -> usually use  
    -> file: ~/.config/git/config  
  c) Local Level: --local option. Specific to the current repository  
    -> file: .git/gitconfig

- Config
```sh
$ git config --global user.name "Hyuna Won"
$ git config --global user.email hyunawon417@naver.com
$ git config --global init.defaultBranch main
```

- Check
```sh
$ git config --list
$ git config --list --show-origin
$ git config user.name
```

3. Initializing a Repository in an Existing Directory
```sh
$ git init
```

4. Checking Repository Status
```sh
$ git status
```

5. Adding a new file to be staged (tracked)
```sh
$ git add [file_name]
```

- Modify a file (add file 1 + just modify file 1: total 2)
```sh
$ nano words.txt
```

- Add a file for committing
```sh
$ git add .
$ git status
```

6. Unstaging a file (--cached: still stay a file own)
```sh
$ git rm --cached [file_name]
```

7. Ignoring a file
```sh
$ nano .gitignore
```
```sh
$ [file_name]
```
![image](https://github.com/wonhyuna/temp-repo/assets/68580694/ce1b232f-25b1-4282-91ee-1300ff96b1b8)

8. Commit
```sh
$ git commit -m "commit message"
```

- commit content until now
```sh
$ git log
```

9. Change branch name
```sh
$ git branch
$ git branch -m master main
$ git status
```
