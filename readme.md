## How to use git

- **in the folder in which you intend to create a project** initialize a new git repo with git init
- run git status

## First Time Git Setup

-setup user.name and user.email

## Git Lingo

- branch - a timeline of your code at any given point
- the default branch is called the main 'branch' or 'master'
- commit - a snapshot of your code at a specific point in time
- in order to track files use, 'git add <name of file>' to track a file
- git add . adds all files in current working directory

## Git Stages

- [ ] tracking
      decide which files will be tracked in this repository
- [ ] staging
      decide what will be commited
- [ ] commiting

## Git Log Explaination

- commit hash - unique value describing our commit
- main/master (or other branch name) - name of the branch on which the commit resides
- HEAD - the eyes of the git staging area. The thing that pops up on your screen
- author of the commit
- date of commit
- commit message
- to get out of having no directory press 'q'

## Connecting Git Repo to GitHub Repo

- create repo on GitHub.com
  - sign in
  - green button
  - give repo name
  - choose visibiliti
  - click create repository
- copy the HTTPS or SSH
- run, git remote add origin <pasted link>
  - 'remote' is responsible for remote repos
  - 'add' adds something
  - 'origin' origin is the name given to the remote repe for reference. Common us is origin or upstream
  - '<link>' is the end point from the GitHub repo
- return back to syntax is a good thing!
- to verify its linked run, git remote -v to see endpoint
- you will see
  - name of the endpoint
  - the endpoint itself
  - fetch and push locations
- in order to push your code run, git push origin <name of branch>
- git push origin main
- git push origin master
- git push origin branch1
- example of untracked changes

## Branches

Git allows you to create branches or alternate timelines. They allow you to create an exact copy of another branch. This way you can tinker with the code without affecting the original code. Great for building features without butting heads with other developers on the project.

- run, git branch, to check which branch you are in
- to creat a new branch - git branch <name of branch> - then switch to branch using, git checkout <name of branch>

[!TIP]
two in one! create a new branch and checkout all at once by using: git checkout -b <name of branch>
for instance: it checkout -b develop, where develop is the name given to the new branch

- will say, "switched to new branch <name of branch>"

## In Other Words

- Make commits on my end that generates a newer and updated position for the head to move to, while the origin/master stays behind with untracked and/or unstaged changes

- Then run, git push origin master to put the changes from that local commit into the shared commit that is the GitHub
