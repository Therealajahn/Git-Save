# Git Save Script 

This repository contains an automation script written in Expect that streamlines the Git workflow. Instead of typing multiple commands and re-entering your GitHub credentials manually, this script handles the full process in one run:

* Adds all changes

* vPrompts for a commit message

* Commits with that message

* Prompts for a branch

* Pushes to the selected branch

* Automatically fills in GitHub credentials (using a stored key)

# Features  

* Interactive prompts for commit messages and branch names.

* Automatic push with stored credentials for convenience.

* Credential management: pulls your GitHub password/token from **~/Documents/key.txt**

* Saves time for quick, iterative commits.

# Requirements  

* Expect must be installed on your system.

* A valid GitHub username and personal access token stored in a file:

* Save your token in **~/Documents/key.txt** (first line only).

* Ensure the file is secured with proper permissions:
  
# Usage
1. Clone this repository and make the script executable:
(it would be good to find your config.fish and put this in the same directory,
it might be **~/.config/fish/config.fish**)
```
git clone https://github.com/YourUsername/git-save.git
cd git-save
chmod +x git-save.exp
```
2. Run the script from your repo root.
```
./git-save.exp
```
3. Follow the interactive prompts:

* Enter your commit message.

* Enter the branch name.

* The script will handle git add, git commit, and git push.
# Polish
1. Find your fish config file (it might be **~/.config/fish/config.fish**)
2. Put your **git-save.exp** file in the same directory
3. Add and alias for the **git-save.exp** file:
```
if status is-interactive
  alias git-save='~/.config/fish/git_save.exp'
end
```
4.Now you can execute the script with:
```
git-save
```
