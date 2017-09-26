# "```git``` - the stupid content tracker"
<details>
<summary>Source</Summary>
<code>man git | sed -n '/NAME$/{n;p;}'</code>
</details>

* Formally described as a "Source Control Manager" or "Version Control System"
  * stores and manages all changes made to files contents.
  * exactly what google docs' "revision history" does, but in a more flexible and larger scale
* Allows groups of people to work on the same documents (not necessarily code)
* Created by Linus Torvalds' when he needed a weeklong vacation from working on the Linux Kernel.
  
## git == ?
  * **g**lobal **i**nformation **t**racker (When you’re in a good mood and it works)
  * **g**0dd4mn **i**diotic **t**ruckload of sh!t (When it breaks)

## Background:
   * A **git repo** is a folder with a “.git” subfolder that contains information about tracked changes among other things.
   * A repo can contain four types of files
      1. Untracked Files: git ignores these
      2. Tracked Files: git tracks changes for these files
      3. Staged Files: these files are on a metaphorical stage; they’re going to be commited soon
      4. Dirty Files: Tracked files that have been modified since git last checked

## Using git and GitHub

### The difference in git and GitHub
git is a command-line based software that facilitates version control. It was first released in 2005.

GitHub is a web-based project that leverages git's functionality and adds its own features. git can be accessed using a terminal emulator. GitHub has its own desktop GUI application and can also be worked on using only its web-app. It was founded on

### Getting Started
  1. *Fork* this repository using the "Fork" button on the top-right. This creates a personal copy of the repository and lets you experiment and test changes without influencing the original repo.
     * Alternately, you can make your own repository from [here](https://github.com/new).
  2. ```clone```
     * ```clone``` your forked repo by typing ```git clone https://github.com/your-username/csc-wksp-git```
     * This creates a local copy of your repository on your computer.
  3. ```status```
     * USAGE: ```git status```
     * You should see:
       > On branch master
       
       > Your branch is up-to-date with 'origin/master'.
       
       > nothing to commit, working directory clean
     * This means that your local copy is up-to-date with the copy that the server has.
  4. Make some modifications to one of the repo's files.
  5. Check the ```status``` again. git will inform you that it has detected a file change.
  6. ```add```
     * USAGE: ```git add [path]```
     * To add all files in the current directory, use ```git add .```; Note that this does not account for deleted files
     * To add ALL tracked files, use ```git add -A```; Note that this does account for deleted files.
  7. ```commit```
     * USAGE: ```git commit -m "short message explaining the changes"```
     * This publishes your code within the local git repository
  8. ```push```
     * USAGE: ```git push -u origin master``` (for the first time) and ```git push``` (subsequently)
     * pushing changes published your code to your GitHub repository.
  9. ```pull```
     * USAGE: ```git pull```
     * If you or a collaborator makes changes to the repository, you should *pull* their changes before working on new changes. This is the best way to avoid *merge conflicts* (when git fails to automatically merge your new code with an older version). Merge conflicts are most commonly the reason git transforms into a truckload of sh!t. 
  
