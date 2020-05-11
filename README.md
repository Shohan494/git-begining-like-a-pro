## lets-git

### 0. we have to create a repository in github, which is optional, we can directly start work in our local machine,
    - inside our work directory, project root we will type - `git init`
    - this will create our git repository from very beginning 
    - we will start work from local master branch (main branch by default)

### 1. you will obviously develop some cool applications or whatever, solve some tough problems through code
    - so you will write code, change them, test them
    - anything you do, you should mark the changes with - `git diff, git log, git status`
    - want to track things by git? start by adding them, each file or all - `git add .` (yes, that's not a period) :smile:
    - what have you done just now after some change, some code editing, can you explain it to yourself?
    - that's commit - `git commit -m "linkin park - what I've done, I'm commiting by myself"`

### 2. so, so far we created git repository in our local machine, and we are working :sunglasses:
    - if we check we will see we are currently working on a branch called master
    - try - `git branch / git remote` command and see what happens
    - okay so, now we are bored, we must try something new, let's create a github repository in github.com and see what it says


#### Get started by creating a new file or uploading an existing file. We recommend every repository include a README, LICENSE, and .gitignore.

#### …or create a new repository on the command line
```
echo "# git-test-repo" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/Shohan494/git-test-repo.git
git push -u origin master
```

#### …or push an existing repository from the command line

```
git remote add origin https://github.com/Shohan494/git-test-repo.git
git push -u origin master
```

    - okay, so they are offering 3 things, we don't like to upload and sit back, and we already done some stuffs locally
    - so the last option is we are interested about now
    - we will - `git remote add origin https://github.com/Shohan494/git-test-repo.git`
    - just done the changes added and commited, because we will try to track small changes which is the best way to use git
    - okay, we kind of added some remote stuffs in the last command. we have to know about what actually happened
    - again let's - `git remote`, we will see something called origin, and that's where our local codes are going to be stored
    - we can try again - `git branch`, we will see the same situation

### 3. Okay, so far so good, we missed something from the last instructions though which was given by github repository
    - let's try - `git push -u origin master`
    - github repository of our so far were having just nothing
    - so if we try like - `git push` instead of - `git push -u origin master`, we will have something like - `git push --set-upstream origin master`, which is actually saying there are currently no master branch in the remote origin
    - after doing so, I mean `git push -u origin master` we will see much like these:

```
To https://github.com/Shohan494/git-test-repo.git
* [new branch]      master -> master
```
    - check your github.com repository, you will find your local repository has been transferred there, nicely
    - just added the changes and - `git commit -m "first time pushing from local master to origin master"`

### 4. Time for some more fun, let's branch
    - try - `git branch -a`, we will see local and origin master from remote
    - we have some options though, but we are always trying to do something from local machine at first
    - so master branch is the default branch for a git repository
    - branching has many purposes and reasons, we create new branch for our own needs and for smarter project source code managing
    - for example we need to do a lot of test, we add new features, while buiding stuffs they crashes, they give errors etc
    - so master branch or main branch is always compared with the good state of a project that can serve it's purposes without any major issue
    - let's create a new branch - `git branch develop`, this will only create a new one based on the current branch we are using
    - check by doing - `git branch`, the star will point your current branch and will also show you the new branch you have just created
    - delete this branch - `git branch -d develop`
    - recreate branch and directly move onto the new branch by - `git checkout -b develop`, you will see:

```
Switched to a new branch 'develop'
```
    - just know that, we have created new branch, and basically it is the clone of local master branch
    - the changes we will do now will only be changed for this 'develop' branch, not in master, that will remain the same
    - for this line we are writing, we will check the changes, and will push this 'develop' branch to remote also
    - by using - `git push -u origin develop`
    - so now we have 2 local and 2 remote branches and so far they are synced with github remote branches

### 5. After we do the push from any other branches rather than master branch, for syncing them again from the github repository, we do pull request
    - from github ui create pull request
    - successfully merge the develop branch with the master branch
    - notice that the remote origin master branch is updated, but our local master remained in the old phase when we created 'develop'
    - for syncing remote master and local master, we have to - `git checkout master` - `git pull origin master`
    - so local master got synced again with origin master, all seems fine

### 6. Release, tag and versioning is really much more fun
    - for example this line is MASTER BRANCH
    - for example this line is DEVELOP BRANCH
    - for example this line is NEW-FEATURE BRANCH
    - for example this is our current RELEASE BRANCH - 1.0.0
    - we did - `git tag 1.0.0` and then - `git checkout develop` and then - `git merge release-1.0.0` and then `git branch -d release-1.0.0`
    - then we pushed the develop to origin develp and then by the same way merged with master
    - we also did something like - `git push --tags`
    - which worked as version release

### 7. Awesome, we made it so far and million more miles to go :rocket:

* main source will be sent/uploaded/synced with github finally

#### Next Phase - A little high level noises they will make
```
notes
restore
reset
rm
mv
```
