# GIT CHEAT SHEET
##### *Week1/Day 1 of the BN Bootcamp we were asked to create a cheat sheet for using terminal/GIT, uploading and downloading code to GitHub*

### BASIC TERMINAL NAVIGATION

- `pwd` → This allows you to find location of current file path 

- `clear` → This declutters your terminal window and allows you to have a cleaner work space

- `ls` → This lists whatever folder or file resides in your current location

- `ls` 'directory_name' → lists whatever folder or file resides in specific directory

- `ls -l` → This gives you extra information of the current contents of your location also known as a flag

- `man ls` → This gives you a directory of flags you can use to help navigate through your directories on Terminal

- `cd 'directory_name'` or `cd Documents/directory_name` → Navigate into desired directory

- `cd` → Takes you back to the beginning of the file tree

- `cd` .. → Allows you to go back to previous directory, *if you would like to go back further use 'cd …' etc.*


### BASIC TERMINAL FILE MANIPULATION

- `mkdir 'directory_name'` → Create a new directory at current location

- `touch 'file_name'.txt` → Create a file at current location

- `open 'file_name'.txt` → Opens file for you to view/use

- `rm -r  'directory_name'` → Permanently delete specific directory

- `rm  'file_name'.txt` → Permanently delete specific file

- `mv 'file_name'.txt 'directory_name'`  → Move file to a specific directory

- `mv 'file_name'.txt ..` → Moves file up a directory **(use more < . > to move up more directories)**

- `mv 'file_name'.txt 'file_name01'.txt` → Renames specific file

- `cp 'file_name'.txt 'directory_name'` → Makes a copy of mentioned file to a specific directory


### CREATING A VERSION CONTROL SYSTEM - GIT

- `git init` → Create a repository (history) *FIRST STEP DO NOT MISS*

- `ls -a` → Allows you to check if there is a new git directory created; *directory will end with '.git'*

- `git status` → Allows you to view a brief summary of what has been modified or added/tracked in git directory

- `git add 'file_name'.txt` → Track a specific file

- `git add .` → Stages all changes in the current directory **(make sure to use this before commit)**

- `git commit -m "current level working on file"` → Creates a record of the current stage of the file that you are working on so you can track back later to it if required. *Allows you to add description of current stage between the " "*

- `git log` → Shows you a detailed list of commits made so far **(good for checking which stage to track back to or what commits have been made so far)**

- `git revert ab12345` → This will undo a specified commit *(use 'git log' to get first seven characters of the commit's ID to specify on this command)* **NOTE: This will only undo the specified commit and not every commit after it so any code reliant on the code inside this commit will not function.**

- `git reset ab12345` → This will undo the specified commit and every commit created after it 

- `git rebase ab12345` → This will undo and completely remove the specified commit and every commit after it from the history


### UPLOADING REPOSITORY TO GITHUB

- `git remote add origin 'githuburl.git'` → This links the local git repository to the GitHub account **(make sure to copy in the SSH link from the GitHub repositry)**

- `git push origin main` → This uploads the code to GITHUB


### DOWNLOADING REPOSITORY FROM GITHUB

- `git clone 'desiredrepository/githuburl.git'` → This clones a repository from GitHub. **NOTE: MAKE SURE YOU HAVE 'cd' TO BEGINNING OF FILE TREE AND YOU ARE NOT CLONING IT ONTO ANOTHER REPOSITORY**

- `git pull origin main` → This downloads any changes made by the author or anyone else using the repository
