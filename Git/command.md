# create a new repository on the command line

### echo "# practice" >> README.md
### git init
### git add README.md
### git commit -m "first commit"
### git remote add origin https://github.com/gowtham551/practice.git ---versioning
### git push -u origin master   --the data from local repo to remote repository
### git pull    --the data from remote repo to local repo
### git status  --to get weather the file is in tracked or untracked
### git fetch origin <commit id> --to get a specific version or file data
### git checkout FETCH_HEAD --to get the data

---config git---

### git init
### ls
### ls -a
### git config --global user.name"gowtham551"
### git config --global user.email"gowtham.konchada1508@gmail.com"
### git config --list   --display all configured list files

---push an existing repository from the command line---

### git remote add origin https://github.com/gowtham551/practice.git
### git push -u origin master

# 3 stages in Git

### i. workspace          (git status - display untracked files info and the file in red colour)
###    git add -A/./*    (move all files in workspace to staging/index area)
###    git add filename  (move particular file workspace to staging/index area)
###    git status
### ii. staging/index area (git status - display tracked files info and the file in green colour)
###     git commit -m "save name"(move data from staging/index area to local repository) --(-m=message)
###     git status  
### iii. local repository   (git log)
###      git push -u origin branch name (move data from local to centralized repository)

# commands

### git log (display commit id info)
### git log --oneline (display commit-id with 1st 7 characterstics and all commit id info display in one line
### git log -2 (display latest 2 commit id's)
### git log --oneline -2 (latest 2 commit id's display in short format)
### git log --author=name
### git log --until=yyyy-mm-dd (it will display log's upto that date)
### git log --oneline --decorate   

---forward the data from workspace to local repo---

### workspace --> staging or index area == git add .
### staging --> local repo == git commit -m "desc"

---backword the data from localrepo to workspace---

### local repo --> staging or index area == git reset --soft cid(commit id)
### staging --> workspace == git reset head filename
### local repo --> workspace == git reset --mixed cid (backword data from local_repo to workspace)

# git branches
  Here by default branch name is "master"
### git branch (showing list of git branches available in repo)
### git branch branchname (creating a git branch)
### git checkout branchname (changing from one branch to other branch)
### git checkout -b branchname (create branch instantly and move to that branch)

--- create a branch---

### git branch gowtham (created branch name as gowtham)
### git checkout gowtham (changing branch "master" to "gowtham")
### git merge master (all files in master branch copied into gowtham branch)
### git push -u origin gowtham (push data into github gowtham branch)






