## Git Remotes 
## Push & Pull -- Git Remotes!
## Level 1 Our Command to create remotes

![alt text](image.png)

```
$ git clone
```
## Level 2 Git Remote Branches

![alt text](image-2.png)
```
$ git commit
$ git checkout o/main
$ git commit
```
## Level 3 Git Fetch

![alt text](image-3.png)

```
$ git fetch
```
## Level 4 Git Pull

![alt text](image-4.png)

```
$ git pull
```
## Level 5 Simulating collaboration

![alt text](image-5.png)

```
$ git commit
$ git clone
$ git branch -f main c1
$ git commit
$ git fetch
$ git merge o/main

```

## Level 6 Git Push

![alt text](image-6.png)
```
$ git commit
$ git commit
$ git push
```
## Level 7 Diverged Work

![alt text](image-7.png)

```
$ git clone
$ git fakeTeamwork main 1
$ git commit
$ git pull --rebase
$ git push
```

## Level 8 Remote Rejected!
![alt text](image-8.png)
```
$ git branch feature
$ git checkout feature
$ git push
$ git branch -f main c1

```
