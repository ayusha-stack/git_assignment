**1. Can we have a global .gitignore?**
Git do allow us to define a global gitignore file that lists the files that can be ignored in all repos and new.

**2. How to find difference between two commits ?**
"git diff" command followed by the commit hashes can be used to compare two commits in Git from where we can find the difference.

**3. Write difference between git add and git commit commands?**
git-add : it adds the changes from working directory to staging area which basically means Git tracks changes made in the files but does not commit it into git repository.
git-commit : it takes the changes in staging area and permanently saves them to the git repository.

**4. How to unstage file ?**
To unstage the file in git we can simply use 'git reset "file_name" ' command or simply use 'git restore --staged "file_name".
To unstage all the files at once we can use "git reset"

**5. How to revert a commit ?**
To revert a commit we can use git revert followed by hash of the given commit .
For example: We have the hash of the commit as 123acd. To revert this commit we can simply use:
'git revert 123abcd'

**6. Difference between revert and reset?**
revert: revert undo the changes made by a previous commit and one can see both the original commit and the new revert commit in Git log. Useful for the case where one do not want to delete original commits but want to undo changes.
reset: reset is used to undo changes to the repository, where commit history is changed. Reset is useful to undo changes and start over from the previous commit.

**7. Write the difference between fetch and pill command?**
fetch: This is the command which is used to retrieve the changes made in the remote repository without merging them into local repository. It updates the remote traching branches, but does not modify the local branches.

pull: This is the command which retrieves new changes from the remote repository and merges them into the local branch.

**8. How to handle merge conflicts?**
General approach to handling merge conflicts are as follows:-
>Pulling the changes from the remote repository.
>Identifying the conflicting files
>Resolving the conflicts manually and decide which changes to keep.
> Adding the resolved conflicts and committing the changes and pushing the changes.

