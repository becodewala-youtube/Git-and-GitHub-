
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
## 4) Repository
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
## 5) Staging Area

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
