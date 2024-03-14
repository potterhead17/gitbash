# opening file on vscode

```
git clone https://gitexercises.fracz.com/git/exercises.git  
cd exercises  
git config user.name "sonia"  
git config user.email "soneya17x@gmail.com"  
./configure.sh  
```
# Master
starting the exercise and pushing by verifying 
```
git start  
git verify
```

# Commit-one-file
there are two files in directory, to commit one file, first we have to add it in stagging area and then commit it.
```
git add A.txt
git commit -m“changing one file”
```
# commit-one-file-stagged
both files are stagged, so we can commit one by the given command having file name in the end.
```
git commit -m “one stagged file” A.txt
```
# ignore-them
first, we create a .gitignore file and add all the extentions we want to ignore (*.exe, *.o, *.jar, libraries/ )
```
touch .gitignore
git add .
git commit -m“ignore”
```
# Chase-branch
first, we have to check on which branch we are, and then we have to merge it
```
git branch
git merge escaped
```
# Merge-conflict
first, we have to open text editor to make it interactive. Then, see the content and delete unnecessary info.
```
vim equation.txt
cat equation.txt
git add .
git commit -m“merge-conflict”
```
# Save-your-work
first, we have to save the current work without commiting, then open the file and remove bugs, then go back to our saved work and add the new line.
```
git stash
cat bug.txt
git add .
git commit -m“bug fixed”
git stash pop
cat bug.txt
git add .
git commit -m“line added”
```
# Change-branch-history
we have to use this command which changes the history
```
git rebase hot-bugfix
```

# Remove-ignored
```
git rm ignored.txt
git add .
git commit -m“ignore”
```
# Case-sensitive-filename
```
git mv FILE.txt file.txt
git commit -m“name changed”
cat file.txt
git add .
git commit –amend -m “Add Hello world”
```
# Forge-date

```
git commit –amend –no-edit –date= “1987-01-01”
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
