## Advanced Topics
## Level 1 Rebasing Multiple Branches
![alt text](image.png)
Changed the order such as rebased the branches.

```bash 
$ git checkout bugFix
$ git rebase -i c2
$ git checkout c4
$ git rebase -i bugFix
$ git checkout C5
$ git rebase c4
$ git checkout c6
$ git rebase c5
$ git checkout c7
$ git rebase c6
$ git branch -f main c7
```

## Level 2 Specifying Parents
Git will normally follow the "first" parent upwards from a merge commit, but specifying a number with ^ changes this default behavior.
```bash
git checkout main^
```
above will direct to the first parent, ^2, will lead to upward parent. 
![alt text](image-1.png)
```bash
$ git branch -f bugWork c2
```
## Level 3 Branch Spaghetti
Updated these three branches with modified versions of the last branch.
![alt text](image-2.png)
```bash
$ git checkout one
$ git cherry-pick c4 c3
$ undo
$ git cherry-pick c4 c3 c2
$ git checkout two
$ git cherry-pick c5 c4' c3' c2' 
$ git branch -f three c2
```