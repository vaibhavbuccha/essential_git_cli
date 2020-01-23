# Essential git commands for version control. 

### Version Control :- Version control systems are a category of software tools that help a software team manage changes to source code over time. Version control software keeps track of every modification to the code in a special kind of database. If a mistake is made, developers can turn back the clock and compare earlier versions of the code to help fix the mistake while minimizing disruption to all team members.

 - for clone a repository from the remote repository we have to use clone command.

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
- for check all the commit history we have to use log command .
```bash
git log 
```

- for create a new merge request or branch .

```bash
git branch <branch name>
```

- push code to an specific branch
```bash
git push origin <branch name>
```