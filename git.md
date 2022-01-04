# Git 


 
Git is a Distributed Version Control systems (DVCS) that stores data ina file system in a series of snapshots
 
 
## Lets talk version control
This allows you to revert files back to pervious versions. You can track and modify files as well as compare changes making it easy to fix mistakes
 
## Local vs Centralized vs Distributed
 
- Local Version Control systems
  - Means files are on one database
- Centralized Version Control System (CVCS)
  - Files stored on a server for easier collaboration
- Distributed Version Control systems (DVCS)
  - Allows for multiple mirrored repos, less chance of failure and down time.
 
 
 
## Git relies on local resources
 - Every change on any file is tracked by git
 - Makes minimizes the possibility of damaged or lost data
 
## States of Git
 
- **Committed**
  - Data stored on local database
 
- **Modified**
  - Files have been changed but not committed
 
- **Staged**
  - File has been flagged to be committed to snapshot



## Git Workflow

### Git repo has three components
	
1. The working directory (where the files are stored)
1. Index (Area used for staging)
1. Head (points to to the most recent commit

## Saving changes

### Tracked vs untracked

- Tracked
  - These files can be modified, unmodified, or staged because they were part of the most recent snap
- Untracked
  -  Files that were not in the most current snapshot

## Git life style

After file is edited git flags file
You stage the edited file
You commit stage changes

<!-- **Git commands**
  - git status
  	 - git add filename
-   Track one file
	-   Git add
-   Track all files
	-   Git commit -m “ files notes”
Commit multi files with same notes
	Git commit -a
Commits  a snapshot to all mods to tracked files in directory 
-->