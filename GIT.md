
# Git Setup

After Installing git, set it up with your username and email address. To do so, open a terminal/shell, I recommend the one in the git app and type:
For your name:

`git config --global user.name "Your name here"`

For your email address:

`git config --global user.email "your_email@example.com"`

Don’t type the $; that just indicates that you’re doing this at the command line

## How to Commit

Initialize a git repository in a folder:

`git init`

Add everything to a commit:

`git add .`

Add your Commit Message:

`git commit -m "Initial Commit"`

Specify the branch you want to push to:

`git branch -M main`

Add the url of the repository you wanna push to:

`git remote add origin https://github.com/yourusername/yourrepositoryname.git`

Finally, push!

`git push -u origin main`

## Push to an existing repository

Add the url of the repository you wanna push to:

`git remote add origin https://github.com/yourusername/yourrepositoryname.git`

Specify the branch you want to push to:

`git branch -M main`

Finally, push!

`git push -u origin main`

## How to keep a local repository and an online one up to date

Pull with rebase:

`git pull --rebase`

Push!

`git push -u origin main`

## Clone a repository

Navigate to the main page of the repository.
Above the list of files, click  Code.
To clone the repository using HTTPS, under "Clone with HTTPS", click the copy button. To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click the copy button. To clone a repository using GitHub CLI, click Use GitHub CLI, then click the copy button.
Open Git Bash.
Change the current working directory to the location where you want the cloned directory.
Type:

   `git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY`

Press Enter to create your local clone.

## Miscelleanous

[Source](https://kbroman.org/github_tutorial/pages/first_time.html)
