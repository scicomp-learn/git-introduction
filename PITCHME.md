# Versioning with Git

---
@transition[fade-in fade-out]

@snap[north span-30]
<h2> Versioning your code </h2>
@snapend

@quote[If your code runs, don't touch it.](Anonym)

+++
@transition[zoom-in zoom-out]

@snap[north-west]
<h3> What does it mean by _versioning_? </h3>
@snapend

In a nutshell, versioning is a technique for managing large/small projects.

@fa[code-fork]

@ul
- track and documenting changes
- troubleshooting
- adding features
@ulend

---
@transition[fade-in fade-out]

@snap[north]
<h2>What is Git?</h2>
@snapend

@fa[git] is a tool to manage your projects that provides automatic way to track changes in software projects, giving creators to:
@ul

- view previous versions of files and directories
- develop speculative features without disrupting the main development
- back up project and its history securely
- collaborate easily and conveniently with others

@ulend

+++
@transition[zoom-in zoom-out]

@snap[north-east]
<h3>Git Installation</h3>
@snapend

Follow instruction for installation in [README](https://github.com/sk-datascience/git-introduction/blob/master/README.md).

+++
@transition[zoom-in fade-out]

### Git Configuration

```bash
$ git config user.name "Your Name"
$ git config.user.email "your.email@example.com"
$ git config
$ git help
```

@[1-2](Configure your name and email)
@[3](Show all git configuration option command)
@[4](Show common git commands)

---
@transition[fade-in fade-out]

@snap[north]

<h2>Getting Started</h2>

Outline:

@ol
- @size[0.8em](Initiate your git repository)
- @size[0.8em](Just code!)
- @size[0.8em](Saving changes)
- @size[0.8em](Status and log)
- @size[0.8em](Undoing changes)
- @size[0.8em](Collaborating with: `remote`, `fetch`, `push`, `pull`)
- @size[0.8em](Branching)

@olend

---
@transition[fade-in fade-out]

@snap[north-east]
<h2>Initiate git _repository_</h2>
@snapend

> Repository is just a fancy term for a Directory. A virtual storage for saving versions of your code, which can be accessed when needed

+++
@transition[zoom-in zoom-out]

Initiate git repo by:

```bash
$ mkdir YourProjectName && cd YourProjectName
$ git init
Initialized empty Git repository in Users/name/YourProjectName/.git/
```

@[1](Create project directory)
@[2](Initate as Git Repository)
@[3](Yes you're doing good!)

+++
@transition[zoom-in zoom-out]

### Or

@quote[You can use the `demo-project` instead for convenience]

+++
@transition[zoom-in fade-out]

### Then, JUST CODE!

code with your favorite programming language

_or_

play around with 3 files in the `demo-project`

---
@transition[fade-in fade-out]

## Git States

![Git State](template/images/git-states.png)

+++
@transition[zoom-in zoom-out]

### 3 States

1. Working directory
2. Staging area
3. (.git) Repository

+++
@transition[zoom-in zoom-out]

### Working Directory

May consist of __untracked__ files and also __unstaged__ files. It's just your
"local working directory"

+++
@transition[zoom-in zoom-out]

@quote[ To be able to track changes, you need to specify what files need to be tracked in a `.git` repo](author)

+++
@transition[zoom-in zoom-out]

If you're just initiate a git repository, and type command `git status`, then you will get

```git
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
```

+++
@transition[zoom-in zoom-out]

### Meanings?

@ol
- You don't have any commits yet
- You have nothing to commit (cause you haven't tracked any files)
- "So, track one"
@olend

---
@transition[fade-in fade-out]

## RECAP

@ol
- We have **initiate** our first git repository (with `git init`)
- Make changes in the codes (demo-project or your own codes)
- First attempts with `git status` (for?)
- Understand the difference between local directory and git repository
- **Next:** Staging, Saving changes, Status, and Log
@olend

---
@transition[fade-in fade-out]

## Staging

Staging is a process of versioning in git where files are added to stage area
(files are *staged*) and prepare them to be committed and save the changes in
git repo

+++
@transition[zoom-in zoom-out]

### Important Terms

**Untracked:** Changes are not tracked

**Unstaged:** These aren't part of git repo

+++
@transition[zoom-in zoom-out]

### Notes

@quote[Saving the changes of codes doesn't mean saving the version of the code](beware!)

+++
@transition[zoom-in zoom-out]

### Workflows

![staging](template/images/sk-datascience_git-intro_staging.png)

+++
@transition[zoom-in zoom-out]

### Hands-On

```bash
$ git status
$ git add FileName.whatever
$ git status
```

@[1](Shows git state of the working directory)
@[2](Add/stage/track files in staging area and prepare to be commited/saved)
@[3](Shows git state after adding the files)

+++
@transition[zoom-in fade-out]

### Similar Comands

```bash
$ git add .
```

@[1](Add all files, literally everything in the directory, to staging area)

+++
@transition[zoom-in zoom-out]

```git
...something else...

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   demo.py
```

@[1](other info)
@[3-6](main information of your added/staged files)

---
@transition[fade-in fade-out]

## Commit

Coming Soon..

---
@transition[fade-in fade-out]

## Reference

[Udacity - Version Control with Git](https://www.udacity.com/course/version-control-with-git--ud123)

[Medium - Basic Tutorial Git](https://medium.com/ai-saturdays/basic-tutorials-part-2-ee778e5926cf)