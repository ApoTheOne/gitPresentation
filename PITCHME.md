# MARKDOWN

# Why _you_ should use Markdown to write your next blog post

[Markdown][1] is just lit, it will make your _whole life_ easier. **I promise.**

[1]: http://github.com/apotheone

# GIT CLI BASICS

##### CONFIG & HELP

To list all config:

```
git config --list
```

##### To get help:

git < verb > --help  
git help < verb >

```
git help config
git add --help
```

---

#### Add existing code base to GIT source control

##### Initialize a git repo:

```
git init
```

List all files in current directory

```
ls -la
```

To remove git tracking

```
rm -rf .git
```

---

##### Adding files to staging

```
echo 'useless text' > useless.txt
```

git add < fileName >

```
git add useless.txt
git add .
git add -A
git status
```

---

To unstage a file

git reset < filename >

```
git reset useless.txt
```

To unstage all files:

```
git reset
```

---

Commit files

```
git add -A
git commit -m "Initial commit"
git status
git log
```

---

Avoiding files to be tracked by GIT source control using .gitignore
//touch .gitignore
echo 'useless.txt' > .gitignore
git status

```
git add .gitignore
git commit -m "Added .gitignore file in the project"
git status
```

---

Sets the new remote

```
git remote add origin remote repository URL
```

Verifies the new remote URL

```
git remote -v
```

Add, commit, pull and push

```
git push origin master
```

Add, commit, pull and push

```
git add .
git commit -m "updated readme.md"
git pull origin master
git push origin master
```

---

##### Cloning a repo

```
git clone < url > < path >
```

Create a folder and clone existing repo in that folder:

```
git clone ../remote_repo.git
```

Go to a new folder and clone a repo from Github

```
git clone https://github.com/apotheoun/gitPresentation.git .
```

---

##### Remote branch and branch info

```
git remote -v
git branch -a
git branch -r
```

---

git branch name
git branch
