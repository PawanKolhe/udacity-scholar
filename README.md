# udacity-scholar
Please read the following instructions on how to create pull request to this repo

**Step 1. Fork Repository**
```
From the upper-right corner, click on 'Fork', please make sure you are logged in to your GitHub account
```

**Step 2. Clone Repository locally**
Once it has been forked, you have full control over it, clone it locally so you can work on it
for example, I will clone it locally like this:
```
$ git clone https://github.com/<your-github-username>/udacity-scholar.git
$ git clone https://github.com/abidmunirmalik/udacity-scholar.git
```

**Step 3. Create Upstream to remote original**
Besides cloning your forked repot, we need to create a handle to original repo (from where we forked)
```
$ git remote add upstream https://github.com/clouddevopsdba/udacity-scholar.git
```

At this point, our local prompt should look like this:

```
$ git remote -v
origin	https://github.com/abidmunirmalik/udacity-scholar.git (fetch)
origin	https://github.com/abidmunirmalik/udacity-scholar.git (push)
upstream	https://github.com/clouddevopsdba/udacity-scholar.git (fetch)
upstream	https://github.com/clouddevopsdba/udacity-scholar.git (push)
```

**Step 4. Pull from Community branch to be in sync with udacity-scholor repo**

```
$ git pull upstream master
```

**Step 5. Update your remote master with any updates coming from upstream**

```
$ git push origin master
```


**Step 6. Checkout your own branch and create your file for PR (Pull Request)**

```
$ git checkout -b iam-udacity-scholar
Switched to a new branch 'iam-udacity-scholar'
malik@goobunta:~/git/udacity-scholar$ git branch
* iam-udacity-scholar
  master
```  
**Step 7. Create file and commit the change to your local branch**

```
$ touch abid.udacity
$ git add abid.udacity && git commit -m "added file"
```

**Step 8. Merge your local branch to your local master**

```
$ git checkout master && git merge iam-udacity-scholar && git branch -d iam-udacity-scholar
```
