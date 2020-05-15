# git branching is a very powerfull thing and its also supper amaizing

> show all branches

```bash
git branch
```

> show your current branch
```bash
git branch --show-current
```

> switch to another branch
```bash
git checkout <branchname>
```

> create and switch with in single command
```bash
git checkout -b "branchname"
```

> git create branch
```bash
git branch <branchname>
```

> Delete branch
```bash
git checkout -D  "branchname"
```
- [x] There are 2 ways to destroy a brach one is using *-D* flag and another one is *-d* flag now the diffrence between both is that *-d*  will give an error if there any commit is pending but *-D* don't give any error it directly delete the branch.

```bash
git checkout -d  "branchname"
```