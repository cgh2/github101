## common git misktake

#### spell last commit message wrong
```
git commit --amend #rewrite the commit message

git commit --amend --no-edit #modified the wrong part but the commit message keep the same

```

#### splling mistake on branch name
```
git branch -m feature-brunch feature-branch

# if your have already pushed this branch(feature-brunch)
git push origin --delete feature-brunch
git push origin featur-branch
```

#### accidentally push all changes to the  master brance
```
git brance feature-branch
git reset HEAD~ --hard
git checkout feature-branch
```
#### forget to add a file to the  last commit 
```
git add missed-file.txt
git commit -amend
```
#### add a wrong file in the repo
```
#if the  file only in staging area but not commit
git reset wrong-file.txt

# if the file had been commit
git reset --soft HEAD~1
git reset wrong-file.txt
rm wrong-file.txt
git commit
``` 
