## To Origin And Beyond -- Advanced Git Remotes!
## Level 1 Merging feature branches
![alt text](image.png)
```
$ git checkout main
$ git pull --rebase
$ git checkout side1
$ git rebase main
$ git checkout side2
$ git rebase side1
$ git checkout side3
$ git rebase side2
$ git checkout main
$ git rebase side3
$ git push
```

## Level 2 Merge
![alt text](image-1.png)
```
$ git checkout main
$ git pull
Fast forwarding...
$ git merge side1
$ git merge side2
$ git merge side3
$ git push
```
## Level 3 Remote tracking branches

![alt text](image-2.png)

```
$ git checkout -b side o/main
$ git pull
$ git commit
$ git rebase -i c2
$ git push
```

## Level 4 Push Arguments
![alt text](image-3.png)
```
$ git push origin foo
$ git push origin main
```

## Level 5 <place> Argument details
![alt text](image-4.png)
```
$ git push origin main^:foo
$ git push origin foo:main
```
## Lvele 6 Git fetch Arguments
![alt text](image-5.png)

```
$ git fetch origin c6:mai
$ git pull origin c3:foo
$ git merge main
$ git branch -f foo c7
$ git checkout foo
```
## Level 7 Oddities of source
![alt text](image-6.png)
```
$ git push origin :foo
$ git fetch origin :bar
```

## Level 8 Git Pull Arguments
![alt text](image-8.png)
```
$ git pull origin c3:foo
$ git pull origin c2:side

```


