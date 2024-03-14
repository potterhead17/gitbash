# opening file on vscode

```
git clone https://gitexercises.fracz.com/git/exercises.git  
cd exercises  
git config user.name "sonia"  
git config user.email "soneya17x@gmail.com"  
./configure.sh  
```
# Master
```
Git start  
Git verify
```

# Commit-one-file
```
Git add A.txt
Git commit -m“changing one file”
```
# commit-one-file-stagged
```
Git commit -m “one stagged file” A.txt
```
# ignore-them
we will write all the extentions we want to ignore (*.exe *.o *.jar libraries/ )
```
Touch .gitignore
Git add .
Git commit -m“ignore”
```
# Chase-branch
```
Git merge escaped
```
# Merge-conflict
```
Vim equation.txt
Cat equation.txt
Git add .
Git commit -m“merge-conflict”
```
# Save-your-work
```
git stash
Cat bug.txt
Git add .
Git commit -m“bug fixed”
Git stash pop
Cat bug.txt
Git add .
Git commit -m“line added”
```
# Change-branch-history
```
Git rebase hot-bugfix
```

# Remove-ignored
```
git rm ignored.txt
Git add .
Git commit -m“ignore”
```
# Case-sensitive-filename
```
Git mv FILE.txt file.txt
Git commit -m“name changed”
Cat file.txt
Git add .
Git commit –amend -m “Add Hello world”
```
# Forge-date

```
Git commit –amend –no-edit –date= “1987-01-01”
```
# Fix-old-typo
```
git rebase -i
vim file.txt
git add .
git commit –ammend
git rebase –continue
vim file.txt
git add .
git commit -m“conflict resolved”
```
