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

* main source will be sent/uploaded/synced with github finally

A little high level noises they will make
```
notes
restore
reset
rm
mv
```
