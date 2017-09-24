# "```git``` - the stupid content tracker"
<details>
<summary>Source</Summary>
<p>``` man git | sed -n '/NAME$/{n;p;}' ```</p>
</detials>

* Formally described as a "Source Control Manager" or "Version Control System"
  * stores and manages all changes made to files contents.
  * exactly what google docs' "revision history" does, but in a more flexible and larger scale
* Allows groups of people to work on the same documents (not necessarily code)
* Created by Linus Torvalds' when he needed a weeklong vacation from working on the Linux Kernel.
  
## git = ?
  * "_g_lobal _i_nformation _t_racker" (When you’re in a good mood and it works)
  * "_g_*dd*mn _i_diotic _t_ruckload of sh*t" (When it breaks_

## Background:
   * A **git repo** is a folder with a “.git” subfolder that contains information about tracked changes among other things.
   * A repo can contain four types of files
      1. Untracked Files --- git ignores these
      2. Tracked Files --- git tracks changes for these files
      3. Staged Files --- these files are on a metaphorical stage; they’re going to be commited soon
      4. Dirty Files --- Tracked files that have been modified since git last checked

## Using git

git is the command line interface. To execute the following commands, you will need to use a terminal emulator.

  1. init
    * Create an empty Git repository or reinitialize an existing one
  2. status
  3. add
  4. commit
  5. log
  6. push
  7. pull
