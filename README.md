# rats_and_cats
VGDC fall game jam 2024 rats and cats



## How to use github 101 and git in general
## TLDR give me a [cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf)
## Basic git
### Cloning the repo on your computer
* Click on the green code dropdown, and copy the link
* From the terminal, git bash, or equivalenet
* Navigate to the directory you want the repo
* type this command ```git clone <the copied link>```

### Adding a file for tracking on the repository
* Make sure the file is in the repository directory or a subdirectory
* Run the command ```git add <your file> ```
* Now your file is tracked

### Making git commits to save changes in the repo
* Make sure the changes are tracked by running the command ```git status``` if you see your file is untracked stop and see the instructions on the above heading
* run this command to add changes to all tracked files on the commit and upload a commit message ```git commit -am "<Your message surrounded by quotes>"```
* When typing a message keep it short but descriptive, "made changes" is a bad message "made changes to <file> to resolve <problem>" is  better

### Pulling changes from the remote repository
* To update your local code with changes someone else made you can type ```git pull```
* If you get something that says "up to date" you're all good, if you get something along the lines of "error due to merge" do not panic, but be careful when resolving these conflicts and contact whoever's commit you are conflicted with to resolve it together

### Pushing your changes to remote
* After doing a commit you can use the command ```git push``` to push the changes to the remote repository
* IMPORTANT: this command will not work unless your local branch is up to date you can make sure your branch is up to date by doing ```git pull``` before ```git push```

## More advanced git
### Branches 
* branches are used to divide work based on features or interaction, I have created some general branches, DO NOT PUSH TO THE MAIN BRANCH when working on a feature please :)
* I have made some branches already namely dev (general dev), dev_scav (offshoot of dev_scav), and dev_fight (offshoot of dev_fight)
* To view all branches you have locally run the command ```git branch```
* To make a new branch or get a branch from online, or switch branches do ```git checkout <branch name>``` the names are case sensitive, be careful

### Pull requests
* After you've pushed your completed work or feature to your branch from your local repo go ahead and open a pull request to the branch it was made from (for example dev_scav would make a pr into dev)
* This is complicated from the command line just make PR's from the repository and the pull_request window
* Do not approve your own request, make it and leave it, it is better if somebody else looks at it and approves it

### Issues
* Issues are managed via the issues tab in the repository if there is a task that needs to be done it can be put there and assigned to someone or labeled.
* It would be good to mark major tasks, problems, or jobs with an issue that is assigned to one or more people

### Fixing mistakes
* If you made a mistake and want the original version of a file from a repo you can do ```git checkout <file>```
* If you have really messed up on the local repo you can do ```git reset --soft HEAD~n``` where n would be replaced with how many commits backwards you want to move
* If it is beyond salvaging reclone the repository

### The git stash command (avoiding merges tip 2 after branching)
* If you have made changes and need to pull you can do ```git stash``` to temporarily undo your local changes and then do ```git pull``` to get your changes back right after the pull do ```git stash pop``` to get them back and git should (mostly) automatically be able to merge the files assuming you have not modified the same line of code


  
