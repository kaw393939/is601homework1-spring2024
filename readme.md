# Homework One

For this assignment you need to setup WSL2 on windows 10/11 and install the Ubuntu operating system as seen in the video.  For Macintosh users, you already have linux/unix on your terminal, so you just need to install Git and you can follow the same procedure to generate the GitHub ssh key.  

## Videos
1. [WSL 2 Setup - Part 1](https://youtu.be/JyvEEy9jIjQ)
2. [Completing the Assignment with Command Line Git - Part 2](https://youtu.be/UaW4sT1CHfc)
## Instructions
1. Install WSL2 with Ubuntu linux installed
2. Create a GitHub Account - [Here](https://github.com/signup)
3. Create a folder for projects in your home directory or where you will remember.
4. Create homework 1 folder and go into the folder.
5. Create an RSA key "ssh-keygen -t rsa -b 2048" and add the contents of your public id_rsa.pub file to github in settings -> ssh key area. 
6. Create a branch, and a merge locally as well as on GitHub.
7. Submit a link to your repository with at least 4 nicely made commits that include commits for gitignore and contents for your readme.md file. 

## Commands - No Particular Order
    1.  ls <- List and variations (ls -a, ls -l)
    2.  pwd <- Present Working Directory
    3.  mkdir homework1 <- command to make a homework1 directory
    4.  rm -r homework1 <- Remove homework 1 directory (Needs -r on directories and no -r if its just one file)
    5.  cd homework1 <- Change directory to homework1 (May need to make it again if you deleted)
    6.  git init <- create a git repo
    7.  git status <-Git Status to check what is or is not tracked and what branch your on
    8.  vi .gitignore <- opens vi to edit a .gitignore file and add *.sw* to ignore swap files from vi
    9.  git add .gitignore
    10. git commit -m "added swp files to ignore"
    11. git checkout master
    12. git merge updateReadme
    13. ssh-keygen -t rsa -b 2048  <-Make ssh key and hit enter no passphrase
    14. vi ~/.ssh/id_rsa.pub <-copy the contents of this to github > setting -> ssh keys -> add new key
    15. Go on Github and create a repository for your homework1 
    16. git remote add origin git@github.com:kaw393939/is601homework1-spring2024.git <- replace the remote with the remote address for your own repo
    17. git remote show <- Shows all remotes
    18. git remote show origin <- Shows the details of the remote called "origin"
    19. git push origin master <- Pushes to github 
    20. git checkout -b listInstructions <- creates a branch called listInstructions and checks it out for you
    21. git checkout master <- Switches to master branch
    22. git merge listInstructions <- merges listInstructions branch to the current branch (Check with git status and be on master)
    23. history <- linux command to show history of commands
