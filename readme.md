# Git Complete Notes

* Git is a version control system (vcs).
* with VCS, we can go forward and backward in time.
* we can modify our data withtout loosing any changes.
* Git has to 2 repos
  1. Local Repo
  2. Remote Repo
* 1. Local Repo: Local repo is on our own machine, so we can have direct access to it.
* 2. Remote Repo: It is usually centraized server, and is entirely optional.
     * changes made locally, can save to remote server.

* To work on a project, teammates pull a repo to their local repo from remote repo.
* Once written, they will push remote repo.

  ![image](https://github.com/mahendharkanuganti/git-learning/assets/103086885/8e153ba5-1b77-427c-9a80-461712931b31)

*  Files we worked locally, they first go to staging area. then once we commit, they go to committed files.
*  Git init command initialise the git and creates a hidden file '.git' in the directory.
    ```
    git init
    ```
* 'git status' to check the status of files.
* Storing changes in a local git repo is called commit.
* To add a file into staging area
  ```
  git add file.txt
  ```
* To commit the file which is in staging area
  ```
  git commit -m 'this is just a message'
  ```
  -m option is for 'message'
* before committing chages, git validates who you are ? because all the changes and commits are tracked by git.
* to authenticate yourself to git
  ```
  git config user.name "mahendhar"
  git config user.email "mahendhar@gmail.com"
  ```
* #### commit:
    * A commit stores the copy of the file in its current state.
    * It saves a copy of entire file or a set of files within the '.git' folder.
    * Even the file is corrupted, we can restore it from the '.git' folder.
    * To restore the file.txt
      ```
      git restore file.txt
      ```
    * To commit
      ```
      git commit -m 'type any message here'
      ```
    * 'git commit' - command will open a vi editor to add a message
* As soon as we create a file it will be in a untracked state in 'git status' command.
* 'git add .'  - this command stages all the files at a time which are in the current directory.
* 
  
