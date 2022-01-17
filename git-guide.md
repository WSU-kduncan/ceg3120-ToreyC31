- status
	- Shows status of the local repository. This status includes:
		- number of local commits that have not been synced with remote (GitHub)
          	- list of files in local folder than are NOT being tracked by git
          	- list of files in local folder that have changes that need to be committed
	- Example: git status
- clone
	- Clones a repository into a directory.
	- Example: git clone git@github.com:example/example.git
- add
	- This command adds newly made, or newly changed files from your current directory
          to the cloned repository you currently working from.
	- Example: git add .
- rm
	- removes files from the current repository.
	- Example: git remove example.txt
- commit
	- This commend creates a snapshot of your repository to be listed in GitHub.
	- Example: git commit -m "Updated Example for Readme.md"
- push
	- Pushes the information that was created or changed to the repository that 
          you are working in to send to GitHub.
	- Example: git push
- fetch
	- Obtains all items from the repository that are not currently being used.
	- Example: git fetch origin
- merge
	- This is used to combine branches into one active one.
	- git merge example-branch-here
- pull
	- This is the most common way to update your repository. Git pull updates any information from your current working branch.
	- Example: git pull
- branch
	- This command, pending the version used, will list, create or delete branches.
	- Example to delete a branch: git branch -d example
- checkout
	- Creates a branch, assists to get to said branch.
	- Example: git checkout example-branch
- init (NOT YET)
	- turns any directory or item into a repo
	- Example to turn a directoru into a git repo: git init example-directory-name
- remote (NOT YET)

git files & folders:

- .git folder
	- the folder created once you run git init
- .gitignore file
	- A PT file that contains items to ignore, such as files/directories.
- .git/hooks (NOT YET)

GitHub:

- Pull requests
	- Pull requests lets you tell others about changes you have made in a branch.
- SSH authentication to repositories
- Actions (NOT YET)

