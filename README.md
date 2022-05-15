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
1) Initialize a git repository in a folder:

```
git init
```

2) Add everything to a commit:

```
git add .
```

3) Add your Commit Message:

```
git commit -m "Initial Commit"
```

4) Specify the branch you want to push to:

```
git branch -M main
```

5) Add the url of the repository you wanna push to:

```
git remote add origin https://github.com/yourusername/yourrepositoryname.git
```

6) Finally, push!

```
git push -u origin main
```

<hr>

# Push an existing repository
1) Add the url of the repository you wanna push to:

```
git remote add origin https://github.com/yourusername/yourrepositoryname.git
```

2) Specify the branch you want to push to:

```
git branch -M main
```

3) Finally, push!

```
git push -u origin main
```

<hr>

# How to keep a local repository and an online one up to date
1) Pull with rebase:

```
git pull --rebase
```

2) Push!

```
git push -u origin main
```

# Clone a repository
1) Navigate to the main page of the repository.
2) Above the list of files, click  Code.
3) To clone the repository using HTTPS, under "Clone with HTTPS", click the copy button. To clone the repository using an SSH key, including a certificate issued by your organization's SSH certificate authority, click Use SSH, then click the copy button. To clone a repository using GitHub CLI, click Use GitHub CLI, then click the copy button.
4) Open Git Bash.
5) Change the current working directory to the location where you want the cloned directory.
6) Type:
   ```
   $ git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY
   ```
7) Press Enter to create your local clone.

<hr>
<p>Miscelleanous<p>
<a href="https://kbroman.org/github_tutorial/pages/first_time.html">Source</a>
