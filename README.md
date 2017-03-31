# testing-merge

## Local Environment
```
mkdir testing-merge
cd testing-merge/
git init
git remote add origin https://github.com/ahchienong/testing-merge.git
```


## Creating New File
```
vi test.html
```


## Add and commit the New File
```
git add .
git commit -m "initial commit of test.html"
```


## Push master branch to Remote
```
git push -u origin master
```


## Create new branch from master branch & checkout the new branch
```
git checkout -b new-feature
```


## Add new file & commit to the new branch created
```
vi new-feature.html
git add .
git commit -m "added new features"
```


## Push new-feature branch to remote 
```
git push origin new-feature
git status
```


## Checkout master branch again
```
git checkout master
git status
```


## Editing existing files in master branch & push to remote origin
```
vi test.html
git add test.html
git commit -m "updated test.html to fix bugs"
git push origin master
```

## Checkout new-feature branch again
```
git checkout new-feature
```


## Merge the changes in `master` to `new-feature`
* Objective : To get the changes in `master` in `new-feature`
```
git merge master
```

## Check and push the merged branch back to remote origin
```
git push origin new-feature
```

