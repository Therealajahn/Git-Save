#Git Save Script 

This repository contains an automation script written in Expect that streamlines the Git workflow. Instead of typing multiple commands and re-entering your GitHub credentials manually, this script handles the full process in one run:

Adds all changes

Prompts for a commit message

Commits with that message

Prompts for a branch

Pushes to the selected branch

Automatically fills in GitHub credentials (using a stored key)

#🚀 Features  

Interactive prompts for commit messages and branch names.

Automatic push with stored credentials for convenience.

Credential management: pulls your GitHub password/token from ~/Documents/key.txt.

Saves time for quick, iterative commits.

# 📂 Requirements  

Expect must be installed on your system.

A valid GitHub username and personal access token stored in a file:

Save your token in ~/Documents/key.txt (first line only).

Ensure the file is secured with proper permissions:
