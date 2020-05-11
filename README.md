## lets-git

0. we have to create a repository in github, which is optional, we can directly start work in our local machine
    - git init
    - will create local master branch

1. you will obviously develop some cool applications or whatever, solve some tough problems through code
    - so you will write code, change them, test them
    - anything you do, you should mark the changes - git diff, git log, git status
    - want to track things by git? start by adding them, each file or all - git add .
    - what have you done, can you explain it to yourself? that's commit - git commit -m "linkin park - what I've done, I'm commiting by myself"

2. so, so far we created git repository in our local machine, and we are working
    - if we check we will see we are working on a branch called master
    - try git branch and git remote command and see what happens
    - okay so, now we are bored, we must try something new, let's create a github repository in github.com and see what it says

```
Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

…or create a new repository on the command line

echo "# git-test-repo" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/Shohan494/git-test-repo.git
git push -u origin master


…or push an existing repository from the command line

git remote add origin https://github.com/Shohan494/git-test-repo.git
git push -u origin master
```

    - okay, so they are offering 3 things, we don't like to upload and sit back, and we already done some stuffs locally
    - so the last option is we are interested about now
    - we will - git remote add origin https://github.com/Shohan494/git-test-repo.git
    - just done the changes added and commited, because we will try to track small changes which is the best way to use git
    - okay, we kind of added some remote stuffs in the last command. we have to know about what actually happened
    - again let's - git remote, we will see something called origin
    - we can try again - git branch, we will see the same situation

3. Okay, so far so good, we missed something from the last instructions though which was given by github repository
    - let's try - git push -u origin master
    - github repository is now having just nothing
    - so if we try like - git push instead of git push -u origin master, we will have something like - git push --set-upstream origin master
    - after doing so, we will see much like these:

```
To https://github.com/Shohan494/git-test-repo.git
* [new branch]      master -> master
```
    - check your github.com repository, you will find your local repository has been transferred there, nicely

4. 

* main source will be sent/uploaded/synced with github finally

A little high level noises they will make
```
notes
restore
reset
rm
mv
```
