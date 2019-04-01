# Introduction to Git / GitHub

For your assignments you will work in groups of 3-4 people using GitHub Classroom. Therefore we will give you a **brief** introduction to Git / GitHub that you can start right away. 
If you are interested in learning more about Git / GitHub there are several good tutorials that you can watch in addition (e.g. http://swcarpentry.github.io/git-novice/).

## 1. Install git and create a github account (if you haven't done yet)

### 1.1 Installing Git

- Linux (Debian): 
  ```sh
  sudo apt-get install git 
  ```
- Linux (Fedora):
  ```sh 
  sudo yum install git 
  ```
- Mac: https://git-scm.com/download/mac  
- Windows: https://git-scm.com/download/win

### 1.2 Creating GitHub account

- sign up at www.github.com
- free for public repositories

### 1.3 Configuring Git

To tell Git who you are, set your username and email address in your terminal. Any changes pushed to GitHub will include this information.

```sh
git config --global user.name "[username]"
git config --global user.email "[email address]"
``` 


## 2. Workflow

![](https://www.dropbox.com/s/xz6za1xbm45un02/Screenshot%202019-04-01%2009.18.35.png?dl=1)

### 2.1 Checkout a project

You can clone your repository on GitHub to create a local copy on your computer and sync between the two locations. Repositories consist of a collection of all files and the history of those files.

1. On GitHub navigate to the main page of the repository.
2. Under the repository name, click Clone or download. 
3. In the Clone with HTTPs section, copy the clone URL for the 
repository.
4. Open terminal.
5. Change the current working directory to the location where you want the cloned directory to be made.
6. Type `git clone`, and then paste the URL you copied in Step 2.
   ```sh
   git clone https://github.com/...
   ``` 

### 2.2 Staging and Committing the code

Committing is the process in which the code is added to the local repository. Before committing the code, it has to be in the staging area. The staging area is there to keep track of all the files which are to be committed.
Any file which is not added to the staging area will not be committed. This gives the developer control over which files need to be committed.

Use the following commands for staging a certain file or all files inside your project folder:
```sh
git add <file>
git add .
```

Use the following command to commit staged files to the local repository with a commit message. Enter a relevant commit message to indicate what code changes were done in that particular commit:
```sh
git commit -m "commit message"
```

Alternatively you can directly commit all modified files to the local repository with a commit message:
```sh
git commit -a -m "commit message"
```

### 2.3 Pushing and Pulling 

In order to push all the code from the local repository into the remote repository, use the following command:
```sh
git push <remote> <branch>
```

In order to pull the latest changes from the remote repository into the local repository, use the following command:
```sh
git pull <remote> <branch>
```