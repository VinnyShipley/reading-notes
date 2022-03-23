# Git and You

## **Version Control**

A system that tracks changes done to a file, so users can not only edit the current version, but examine prior versions as well. This is made possible with a series of snapshots. As the files are committed, a snapshot is taken of the file.

## **Stages of Git Files**

Within the system there are three states that files can be: Modified, Committed and Staged

* **Modified**

  * A file is modified when it has been edited but not yet committed to the local database

* **Committed**

  * A file is modified when the changes made to it are saved to the local database

* **Staged**

  * Every file grows up hoping to one day be staged. This means that the file has been has been flagged so that the next time a snapshot of the code is made, the change will be saved in with it

## **Workflow**

As files begin to be manipulated by the user into stages of commitment, a workflow emerges, shown here below:

![Workflow image](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

Once introduced into a file into the system it enters a loop of sorts, starting at: *Consistent from the last snapshot &rarr; being modified by the user &rarr; the user staging the modified file, which then puts it in the newest snapshot &rarr; bringing the file finally back to being consistent with the most recent snapshot*

## **Git Status, My Hero and Yours**

To check the status of the files within your system, simply use the lifeguard command of the Git system: *git status*.

Git status allows the user to track where all modified files are in terms of their position in the workflow. Once the user knows the status of the files, specifically the modified ones, they can...

Add, commit and push the files to incorporate them into the newest snapshot
