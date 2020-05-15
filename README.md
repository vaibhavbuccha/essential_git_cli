# Essential git commands for version control. 

- [x] Version Control :- Version control systems are a category of software tools that help a software team manage changes to source code over time. Version control software keeps track of every modification to the code in a special kind of database. If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake while minimizing disruption to all team members.

 - for clone a repository from the remote repository we have to use clone command. git clone bascically copy the complete reposity.

```bash
git clone <repository_Url>
 ```

 - for check the additions or modification we have to check status command.
 ```bash
  git status 
```
- for adding file we have to use git add command.
```bash
git add
```
> we have to use ( . ) for add all files otherwise we can specify the filenames

- for commiting the changes we have to use commit command .
```bash
git commit -m 'here is the message for the above commit.'
```
> ( -m ) is a flag use for message .

- for pushing the file to the remote we have to use push command.
```bash
git push
```
- [x] GIT LOG
---
- This helps give context and history for a repo.

- for show all logs
```bash
git log 
```
- for git small commit hashes
```bash
git log --online
```

- Get logs before date
```bash
git log -before="date"
```

- Get logs by author
```bash
git logs --author="authorName"
```

---
- for create a new merge request or branch .

```bash
git branch <branch name>
```

- push code to an specific branch
```bash
git push origin <branch name>
```

- set origin to online repository
```bash
git remote add origin <url>
```

- set fast forward push operation
```bash
git push -f origin master
```
- set global user name in git
```bash
git config --global  user.name "username"
```
- set global user email in git
```bash
git config --global  user.name "useremail"
```
- set useremail for non global
```bash
git config  user.name "useremail"
```

- set username for non global
```bash
git config  user.name "username"
```
- get username
```bash
git config user.name
```
- get useremail
```bash
git config user.email
```

- get global username
```bash
 git config --global user.name

```
- get global useremail
```bash
 git config --global user.email

```


- get all latest commits 
```bash
git pull origin <originName>
```

- [x] GIT STASH
---

- Git stash is mainly use to save changes made when they are not in a state to commit them to a repo.

```bash
git stash
```
- for undo the last stash 
```bash
git stash pop
```
- The file or change which are stash are not staggable or trackable in status. for track them we have to use following command.
```bash
git stash list
```

- for inspect them.
```bash
git stash show
```

- If we want to work again with stash changes than we have to use.
```bash
git stash apply
```
---

- For compair 2 commits 
```bash
git diff <commitHash1> <commitHash2>
```

- Show all remotes
```bash
git remote -v
```

- [x] GIT REVERT
---
- git revert is use for rollback to pervious versions.
```bash
git revert <commitHash>
```
- undo the revert
```bash
git revert HEAD
```

- undo a specific commit 
```bash
git checkout <commitHash>
```
- _Note:-_ All reverts can be tracked in logs.

---

- [] GIT REBASE
---
- IT Takes a set of commits ,copies then store them out side your repo.
- It is another way of merging commits.
- It is make to linner sequence of commits.
- Advantage of rebase is that is makes clear our git logs and history.
```bash
git rebase <branch>
```

---

