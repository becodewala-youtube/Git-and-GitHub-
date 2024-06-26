
# GitHub🐈‍⬛
## 1) Installing🔗
- If we installing git for the first time,then we have to add config like name,email-id(like registration)
### How to Config?🤔

 ```bash
  git config --global user.name "vikash kumar"
  git config --global user.email "becodewala@gmail.com"
```
### To check your name or email is connected or not?🤔
 ```bash
  git config --global user.name 
  git config --global user.email 
```
### To edit Config?🤔
 ```bash
  git config --global --edit  
```
## 2) How can we start making projects?🤔
- To make new code in vs code,give the command in terminal
 ```bash
  mkdir letStart  
```
### To get into the file (changing the director)?🤔
 ```bash
  cd letStart  
```
## 3) Repository
- means, a project that can be track with the help of git
- If we want to make this folder an repo the we do
 ```bash
  git init  
```
- to check the status of our file
 ```bash
  git status  
```
- Before we commit something,first we will track 
 ```bash
  git add  
```
- the if want to check our file is tracing or not again we see this command
 ```bash
  git status  
```
- retrieve an entire repository from a hosted location via URL
 ```bash
  git clone URL  
```
## 4) Staging Area💹

- means area where we hold changes before commit

 ```bash
  working directory=>staging area=>git commit=>Repository  
```
- Before final commit we hold the changes. Suppose we have 15 files in our project and we want to commit only 7 files then we put in staging area, then it will be commit.(git add se file staging area mein aa jata hai)

- Now we will commit
 ```bash
  git commit -m "commit message" 
```
- To see how many commit we have done
 ```bash
  git log  
```
- If we do some changes in file(index.html) , we can see and check our file is modified
 ```bash
  git status  
```
- Now We will create one more file (hello.html), If we will pass the command "git status", we can see that
 ```bash
 modified:index.html
 untracked files:hello.html  
```
- To keep in staging area(track) hello.html
 ```bash
  git add hello.html  
```
- If we will do this our hello.html file will be tracked but index.html will not, So if will do some commit it will be in hello.html not in index.html
- To keep all files in staging area
 ```bash
  git add .(dot) 
```
- To comeback to initial commit
 ```bash
  git checkout filepath/branchname 
```
- If we want to go again at same place 
 ```bash
  git checkout master 
```
## 5) Master branch 🧑‍🏫
- master branch is the main branch where we can make many branches
- Now we will create an branch
 ```bash
  git branch vikash
```
- To check how many branches
 ```bash
  git branch 
```
- Now we have two branch vikash and master
- If we want to switch on vikash branch
  ```bash
  git checkout vikash
```
- Another method to create branch
 ```bash
  git checkout -b <branch_name>
```
- Now we will create third file multily.html, now we will check status
 ```bash
  git status 
```
- It will show untracked files multiply.html, so we will add for track 
 ```bash
  git add multiply.html 
```
- then we have commit a message
 ```bash
  git commit -m " write some meaningfull message"
```
- Now We will switch to vikash branch
 ```bash
  git checkout vikash 
```
- But here vikash branch don't know that we have created a new file(multily.html), so Now we will merge to vikash branch
 ```bash
  git merge vikash/multiply
```
## 6) Other Important Command 🧑‍🏫
- unstage a file while retaining the changes in working directory.
 ```bash
  git reset FILE
```
- diff of what is changed but not staged.
 ```bash
  git diff
```
- diff of what is staged but not yet committed.
 ```bash
  git diff --staged
```
- delete the file from project and stage the removal for commit.
 ```bash
  git rm FILE
```
- change an existing file path and stage the move.
 ```bash
  git mv existing-path new-path
```
- show all commit logs with indication of any paths that moved.
 ```bash
  git log --stat -M
```
- add a git URL as an alias.
 ```bash
  git remote add [alias] [URL]
```
- fetch down all the branches from that Git remote.
 ```bash
  git fetch [alias]

```
- merge a remote branch into your current branch to bring it up to date.
 ```bash
  git merge [alias]/[branch]
```
- Transmit local branch commits to the remote repository branch.
 ```bash
  git push [alias] [branch]

```
- fetch and merge any commits from the tracking remote branch.

 ```bash
  git pull

```
- clear staging area, rewrite working tree from specified commit.
 ```bash
  git reset --hard [commit]

```
- Save modified and staged changes.
 ```bash
  git stash

```
- list stack-order of stashed file changes.
 ```bash
  git stash list

```
