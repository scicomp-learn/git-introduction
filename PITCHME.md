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

<h2>Demo Project</h2>

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
$ mkdir MyProj && cd MyProj
$ git init
Initialized empty Git repository in Users/name/MyProj/.git/
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

### Then

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

## Working Directory

May consist of __untracked__ files and also __unstaged__ files. It's just your
"local working directory"

+++
@transition[zoom-in zoom-out]

@quote[ To be able to track changes, you need to specify what files need to betracked in a `.git` repo](author)

---
@transition[fade-in]

## Coming Soon
