# "```git``` - the stupid content tracker"
<details>
<summary>Source</Summary>
<p>``` man git | sed -n '/NAME$/{n;p;}' ```</p>
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

git is the command line interface. To execute the following commands, you will need to use a terminal emulator.

* To create ***a brand new*** repository 
  0. Create the repo on GitHub
     * Creates an empty git repository
     * Skip this step, if you 
  1. clone
     * Creates a local copy (*clone*) of a repository.
     * USAGE:```git clone URL```
     * Clone this repository: ```git clone https://github.com/zorawar87/csc-wksp-git.git```
  2. status
  3. add
  4. commit
  5. log
  6. push
  7. pull
