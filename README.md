# Git Setup
<h1>After Installing git, set it up with your username and email address. To do so, open a terminal/shell, I recommend the one in the git app and type:</h1>
<h3>For your name:</h3>

```
$ git config --global user.name "Your name here"
```

<h3>For your email address:</h3>

```
$ git config --global user.email "your_email@example.com"
 ```
  
#Don’t type the $; that just indicates that you’re doing this at the command line.
<hr>

# How to Commit
<h3>To initialize a git repository in a folder:</h3>
git init
<h3>To add everything to a commit:</h3>
git add .
<h3>Your Commit Message:</h3>
git commit -m "Initial Commit"
<h3>Specify the branch you want to push to:</h3>
git branch -M main
<h3>Add the url of the repository you wanna push to:</h3>
git remote add origin https://github.com/yourusername/yourrepositoryname.git
<h3>Finally, push!</h3>
git push -u origin main
<hr>

# Push an existing repository
<h3>Add the url of the repository you wanna push to:</h3>
git remote add origin https://github.com/yourusername/yourrepositoryname.git
<h3>Specify the branch you want to push to:</h3>
git branch -M main
<h3>Finally, push!</h3>
git push -u origin main
<hr>

# How to keep a local repository and an online one up to date
<h3>To pull with rebase:</h3>
git pull --rebase
<h3>To push!</h3>
git push -u origin main
<hr>
<p>Miscelleanous<p>
<a href="https://kbroman.org/github_tutorial/pages/first_time.html">Source</a>
