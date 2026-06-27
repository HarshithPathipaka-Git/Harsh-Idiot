# 01. Introduction

## What is Version Control?

Version Control is a system that records changes made to files over time. It allows developers to track modifications, restore previous versions, compare changes, and collaborate with others without losing work.

Instead of creating multiple copies like:

- project-final
    
- project-final-v2
    
- project-final-latest
    
- project-final-final
    

Version Control maintains a complete history of every change in one repository.

### Benefits

- Tracks file history
    
- Restores previous versions
    
- Compares changes
    
- Supports teamwork
    
- Prevents accidental data loss
    
- Makes collaboration easier
    

---

## Types of Version Control

There are three main types of version control systems.

### Local Version Control

Stores version history only on your computer.

**Advantages**

- Simple
    
- Fast
    
- No internet required
    

**Disadvantages**

- No collaboration
    
- Easy to lose history if the computer fails
    

---

### Centralized Version Control (CVCS)

A single central server stores the project history. Every developer connects to this server.

Examples:

- SVN
    
- Perforce
    

**Advantages**

- Easy collaboration
    
- Central backup
    

**Disadvantages**

- Server failure affects everyone
    
- Internet connection is usually required
    

---

### Distributed Version Control (DVCS)

Every developer has a complete copy of the repository, including its history.

Examples:

- Git
    
- Mercurial
    

**Advantages**

- Works offline
    
- Faster operations
    
- Better backup
    
- Easier branching
    
- Reliable collaboration
    

Git is a Distributed Version Control System.

---

## Centralized vs Distributed VCS

|Feature|Centralized|Distributed|
|---|---|---|
|Complete history on every computer|No|Yes|
|Offline work|Limited|Yes|
|Collaboration|Yes|Yes|
|Single point of failure|Yes|No|
|Speed|Slower|Faster|

---

## What is Git?

Git is a free, open-source Distributed Version Control System created by Linus Torvalds in 2005.

Git tracks changes made to files, stores project history, allows developers to work on multiple features simultaneously using branches, and makes collaboration efficient.

Git runs locally on your computer and does not require GitHub.

### Git is used for

- Tracking changes
    
- Managing project history
    
- Creating branches
    
- Merging code
    
- Recovering previous versions
    
- Collaborating with teams
    

---

## What is GitHub?

GitHub is a cloud-based hosting platform for Git repositories.

GitHub stores repositories online, making it easy to back up projects, collaborate with others, review code, manage issues, and contribute to open-source software.

GitHub uses Git, but Git and GitHub are different technologies.

---

## Git vs GitHub

### Git

- Version Control System
    
- Installed on your computer
    
- Tracks project history
    
- Works offline
    
- Open source
    

### GitHub

- Cloud hosting platform
    
- Stores Git repositories online
    
- Requires Git
    
- Enables collaboration
    
- Provides Pull Requests, Issues, Actions, Discussions, and more
    

Think of it this way:

Git is the engine.

GitHub is the service that hosts projects using that engine.

---

## Why Developers Use Git

Git solves many common development problems.

Without Git:

- Difficult to track changes
    
- Risk of losing work
    
- Hard to collaborate
    
- Manual file backups
    

With Git:

- Every change is recorded
    
- Previous versions can be restored
    
- Teams can work together
    
- Multiple features can be developed simultaneously
    
- Mistakes are easy to recover from
    

---

## Repository

A Repository (Repo) is the main storage location for a project.

It contains:

- Source code
    
- Project files
    
- Commit history
    
- Branches
    
- Tags
    
- Configuration files
    

Repositories can be stored locally or on remote platforms like GitHub.

---

## Local Repository

A Local Repository exists on your computer.

You use it to:

- Write code
    
- Commit changes
    
- Create branches
    
- View history
    
- Work offline
    

---

## Remote Repository

A Remote Repository is stored on another computer or cloud service such as GitHub.

It allows:

- Backup
    
- Sharing code
    
- Team collaboration
    
- Synchronizing changes
    

---

## Working Directory

The Working Directory is the folder where you actively create, edit, delete, and manage project files.

Every change you make starts here.

---

## Staging Area (Index)

The Staging Area is an intermediate area between the Working Directory and the Repository.

You choose which changes should be included in the next commit.

Not every modified file must be committed immediately.

---

## Commit History

A Commit is a snapshot of your project at a specific point in time.

Every commit stores:

- The changes made
    
- Author information
    
- Date and time
    
- Commit message
    
- Unique commit ID
    

The Commit History is the chronological record of all commits in a repository.

---

## Snapshot Concept

Git stores projects as snapshots instead of complete file copies.

When you commit:

- Git records the current state of your project.
    
- Unchanged files are reused efficiently.
    
- Only new or changed content is recorded.
    

This approach makes Git fast and storage-efficient.

---

## Git Architecture

Git consists of four primary areas:

1. Working Directory
    
2. Staging Area
    
3. Local Repository
    
4. Remote Repository
    

Typical workflow:

Working Directory  
→ Staging Area  
→ Local Repository  
→ Remote Repository

---

## Complete Git Workflow

A typical Git workflow follows these steps:

1. Create or clone a repository.
    
2. Modify project files.
    
3. Check the repository status.
    
4. Stage the required changes.
    
5. Commit the staged changes.
    
6. Push commits to the remote repository.
    
7. Pull or fetch updates from the remote repository.
    
8. Repeat the process throughout development.
    

This workflow forms the foundation of almost every Git-based software project.