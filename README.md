# Understanding Git

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
  - `$ git add *.html` : Add all .html files to index (stage all .html files)
  - `$ git add .` : Add all changed files to index (stage all changed files)
- `$ git rm --cached <file>` or `$ git reset HEAD <file>` : Remove the file(s) from index (unstage the file(s))
- `$ git status` : Check status of working tree
- `$ git commit` : Commit changes in index
  - `$ git commit -m "<your_commit_message>"` : Commit changes in index with a message
- `$ git remote add origin <HTTPS_URL_of_the_remote_repository>` : Adds the your local repository origin to the remote repository.
  - Go the github dashboard in your browser > Create a new repository > Copy the HTTPS URL and use it above
- `git push -u origin master` : Pushes your local repository (master branch) to the remote repository
- `$ git push` : Push changes to remote repository
  - `$ git push origin <branch_name>` : Push changes made in the branch to the remote repository branch
- `$ git pull origin <branch_name>` : Pull latest from the branch of remote repository
  - `$ git pull` : Pull by default from origin master
- `$ git clone <HTTPS_URL>` : Clone remote repository into a new local directory
- `$ git branch` : List all the branches and check which branch you are currently on.
- `$ git checkout -b <branch_name>` : Create a new branch
- `$ git checkout <branch_name>` : Switch to an already existing branch

## Others

- `$ touch .gitignore` : Create a file called .gitignore (Used to list files are not meant to be commited. Refer [here](https://github.com/sahil505/understanding_git/blob/master/.gitignore))
  - `log.txt` : This written inside .gitignore file will ignore the file log.txt from getting staged or commited
  - `*.txt` : This will ignore all .txt files from getting staged or commited
  - `/dir` : This will ignore the complete dir directory from getting staged or commited
- `$ echo "My github username is sahil505" >> README.md` : Creates a file called 'README.md' with text 'My github username is sahil505'

## Contribute

- Please feel free to contribute to this in any manner. Just create a PR ;)
