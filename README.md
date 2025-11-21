# git-github
Step-by-step tutorial demonstrating how to contribute to open-source projects on GitHub by forking a repository, cloning it, making changes, committing updates, and submitting a pull request for review.


## Q1. What is Git?
Ans. Git is a Version Control System.

1. Git is the most popular Version Control System in the world.
2. Git is free and open source i.e. anybody can use it without any cost.
3. Git is fast and scalable (i.e. can be used in smaller as well as larger projects).

## Q2. What is Version Control System?
Ans. Version Control System is a system that helps to track changes in code.

## Q3. What is the use of Git?
Ans. Git is primarily used for 2 purposes :- 

1. To track the history of our project
2. Collaborate (i.e. helps us to work in a team)

## Q4. What is GitHub?
Ans. Github is a website that allows developers to store and manage their code using Git.

## Q5. What is repository?
Ans. We store our project code in Github in the form of folder and that folder is known as repository. Our Github can have multiple folders i.e. multiple repositories.

**We can view the repositories of other people on Github. We can also make copies of repositories of other people and can make changes in it.**

## Q6. How to create Github Account?
Ans. Visit the website [https://www.github.com]. Click on **Sign Up** button to create an account on Github.

## Q7. How to create a repository on Github?
Ans. Visit the website [https://www.github.com]. Click on **New** button to create a repository. 

Upon clicking **New** button, it will going to ask few questions :- 

1. Write the repository name.
2. Write the description (i.e. tell the reason behind creating this repository).
3. Set visibility to public/private. Public means anybody can access this repository. Private means only you can access this repository.
4. Toggle to **ON** to create a README file.
5. Click on **Create Repository** button.


## Q8. What is the first commit in any repository?
Ans. First commit is named as **initial commit**.

**Just like in relationship, first engagement happens then wedding happens. Similarly, in Github first add (i.e. this change is ready to be committed) happens then commit happens.

## Q9. How to setup Git in our local machine?
Ans. 

1. Install VSCode [https://code.visualstudio.com/download]
2. Install Git Bash for Windows [https://git-scm.com/install/windows]
3. Install Terminal for Mac

**Verify** - Run command **git --version** on terminal to check whether Git has been successfully installed or not.

## Q10. How to install Git/Git Bash in our local machine?
Ans. Go to the website [https://git-scm.com/install/windows] to install Git/Git Bash on Windows.

## Q11. How to configure Git?
Ans. Git Configuration basically tells in which Github Account you want to push the changes. Through which email id you want to make changes in repository in Github Account. 

1. git config --global user.name "SakshiRastogi1302"
2. git config --global user.email "sakshi.rastogi1302@gmail.com"
3. git config --list (gives list of email id, user name)

## Q12. What is clone, cd, clear, ls , ls -a, log and status commands.
Ans. These commands are used to make changes from remote[i.e. Github] to local [i.e. laptop/PC].

1. clone - Cloning a repository on our local machine.

    - git clone <- some link ->

2. status - Displays the state of the code

    - git status

3. cd - is used to change the directory i.e. it allows you to go to nested folder.

4. clear - is used to clean the terminal. 

5. ls - is used to list files inside the folder.

6. ls -a - is used to list all files (i.e. hidden and non-hidden) inside the folder.

7. git log - shows all commit messages.

## Q13. What are the different types of status in Git?
Ans. Different types of status are :-

1. untracked - new files that git does not track yet.

2. modified - changed
3. staged - file is ready to be committed
4. unmodified - unchenged


Changed files = modified
New Files = untracked
Add = stagged
Commit = unmodified

## Q14. What are add and commit commands?
Ans. 

1. Add - adds new or changed files in your working directory to Git stagging area.

    - git add <- file name -> (adds specific file to Git stagging area)
    - git add . (adds all new or changed files to Git stagging area)

2. Commit - It is the record of change.

    - git commit -m "some message" (-m refers to commit message and message should be meaningful)

## Q15. What is push command?
Ans. It upload local repo content to remote repo.

    - git push origin main (here origin refers to the repository that we have cloned and main refers to the branch)

## Q16. What is init command?
Ans. It is used to create a new git repo.

## Q17. How to create a folder in VSCode using Git?
Ans. Using mkdir <-folder name-> command. This folder is not a github repo. To make it, run command git init.

## Q18. How to make the local git repository available on Github?
Ans.

1. Create a repository on Github.
2. Run command :- git remote add origin <-link of repository>

## Q19. How to verify remote?
Ans. git remote -v (check which one is the remote repository).

## Q20. How to check in which branch you are?
Ans. git branch

## Q21. How to rename a branch?
Ans. git branch -M main. Always rename master branch with main branch (copy of your repository) as master is not used today.

## Q22. How to set upstream?
Ans. git push -u origin main. If you do so, then you don't have to write origin main again and again as it says that we want to push all changes in origin main.

## Q23. What should be the workflow of local Git?
Ans. We should always create repository on Github and then we should clone it in our local machine instead of doing vice-versa.

1. Create a repository on Github
2. Clone
3. Make changes
4. Add
5. Commit
6. Push

## Q24. List different types of branch commands?
Ans.

1. git branch - to check branch
2. git branch -er
4. git checkout -b <-new branch name-> - to create a new branch
5. git branch -d <-branch name-> - to delete a branch

**A branch highlighted in green is the branch that we are currently in.**

**We cannot delete a branch (feature 2) when we are using that branch or when we are in that branch. In order to delete it, we have to move to another branch.**

## Q25. How to merge code?
Ans. There are 2 ways in which we can merge the code :- 

1. First Way :- 

    * git diff <-branch name-> - To compare commits, branches, files and more.

    * git merge <-branch name-> - to merge 2 branches

2. Second Way :-

    * Create a pull request (it lets you tell others about the changes you have pushed to a branch in a repository on Github.) by clicking on **Compare & Pull Request**. Add a message and click on **Create Pull Request**. If it's ready to be merged directly then click on **Merge Pull Request**. Then, click on **Confirm Merge**.

## Q26. How to fetch content from remote repo to local repo?
Ans. Using pull command

Pull command is used to fetch and download content from a remote repo and immediately update the local repo to match that content.

    * git pull origin main

## Q27. What is merge conflicts?
Ans. An event that takes place when Git is unable to automatically resolve differences in code between two commits.

## Q28. How to undo changes in Github?
Ans. 

1. Staged Changes
    * git reset <-file name-> - used to reset changes in 1 file
    * git reset - used to reset changes in multiple files

2. Committed Changes (for one commit)
    * git reset HEAD~1 (latest commit is HEAD and HEAD`1 says move HEAD 1 step behind).

3. Committed Changes (for multiple commits)
    * git reset <-commit hash->. Write hash value of that commit to which you want to go. This command will make changes in Github.

    * To make changes in VSCode, write git reset --hard <-commit hash->

## Q29. What is fork?
Ans. A fork is a new repository that shares code and visibility settings with the original "upstream" repository. Fork is rough copy.