# understanding_git

A simplified git tutorial

## What is Git?

> A Version Control System (VSC) for tracking changes in computer files.

- Distributed version control system (Decentralized: Users need not be on the same network to access or make changes)
- Coordinatess work between multiple developers
- Who made what changes and when
- Revert back at any point of time to any point of time
- Local and remote [repositories](https://www.google.com/search?q=repository+meaning&oq=repository+&aqs=chrome.2.69i57j0l2j69i60j69i61l2.3466j0j1&sourceid=chrome&ie=UTF-8)

## Concepts of Git

- Keeps track of your code history
- Takes snapshots of your files in the repository
- You decide when to take a snapshot by making a "commit"
- You can visit any sanpshot at any time
- You can stage files before commiting them (commands for all these are explained in detail below)

## Basic Commands

- `$ git --version` : Check the git version
- `$ git init` : Initialize a local git repository
- `$ git add <file>` : Add file(s) to index (stage the file(s))
- `$ git status` : Check status of working tree
- `$ git commit` : Commit changes in index
- `$ git push` : Push changes to remote repository
- `$ git pull` : Pull latest from remote repository
- `$ git clone` : Clone remote repository into a new local directory
