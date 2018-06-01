---?image=https://raw.githubusercontent.com/wiki/gitpitch/gitpitch/images/stunning.png
---
- README Files |
- MARKDOWN |
- GITPITCH 
---
### README
A README is often the first item a visitor will see when visiting your repository. README files typically include information on:

What the project does
Why the project is useful
How users can get started with the project
Where users can get help with your project
Who maintains and contributes to the project
- What is a README file?
- Importance of README files
- Formats - Read.me, Readme.txt, README.md etc.
---
### What?
Markdown is a text-to-HTML conversion tool for web writers. Markdown allows you to write using an easy-to-read, easy-to-write plain text format, then convert it to structurally valid XHTML (or HTML)
---
#### Why Markdown?

Markdown == FAST && EASY


HTML's start and closing tags  
 vs  
Simple text
---
Let's try it out

Use numbers, *, or - to created list items.

Sample:

* First |
* Second |
* Third |
* Fourth |
---
Hyperlinks:
```
[Text] (link)
```
OR
```
[Text][variable]
variable: url
```
[Click here][g]

[g]: wwww.google.com
[1]: https://github.com/ApoTheOne/gitPresentation
---
Adding images :  
?imageUrl

---
### GIT CLI BASICS

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

---

…or create a new repository on the command line

```
echo "# gitPresentation" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/ApoTheOne/gitPresentation.git
git push -u origin master
```

---

…or push an existing repository from the command line

```
git remote add origin https://github.com/ApoTheOne/gitPresentation.git
git push -u origin master
```

…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
