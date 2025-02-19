## Moving Work Around
## Level 1 Git Cherry-pick
Git cherry-pick allows you to copy specific commits to a branch. 
![alt text](image-2.png)


```bash
$ git checkout main
$ git cherry-pick c3 c4 c7
```
## Level 2 Git Interactive Rebase
It simply opens an  UI where you can reorder or drop commits before applying them which amkes more structured .
![alt text](image-6.png)


```bash
$ git rebase -i HEAD~4

```