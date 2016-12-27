#Lession 2 Reflections


_What happens when you initialize a reposity? Why do you need to do it?_

git creates a .git directory where meta data is stored to let git know about the changes
and status of a given repository. You need to do this so that git can track changes and
status of all files in the repository.

* git init : Initializes a repository
* git status: Gives you status of the repo  of a the last change
* git add : adds files to the staging area

_How is the staging area different from the working directory and repository? What value
do you think it offers?_

The staging area is a place the shows you which files will be part of the next commit. It
allows you to see what will be in the commit before actually performing the commit and enables
you to change it before doing the commit.


To diff the files in the workspace to the files in the staging area:

`git diff`

To diff the files in the staging area to the latest files checked into the repository(?)

`git diff --staged`

`git reset --hard`

Remove any changes to any files (not in staging area?)


`git checkout master`

Re-sync to HEAD

_How can you use the staging area to make sure you have one commit per logical change?_

You can run `git add` which will add specific files to the status area and you can run
`git status` to get a report of which files are on the staging area before running 
`git commit`.

To see curent branches: `git branch`

To create a new branch: `git branch easy-mode`

to switch to the branch: `git checkout easy-mode`

_What are some situations when branches would be helpful in keeping your history
organized?  How would branches help?_

You may want to create a branch when you want to make an experimental change to your code
or when you want to add a new feature for a different version of your product. Branches
help because they allow you to make commits to the main-line (master) that are different
than commits to your branches. It also allows you to merge changes between branches and 
the master.


Here is a ASCI text graph of the coins branch and its relationship to the master branch:

	* 8965bd9 bug: Fix issue where you can fire a continuous stream of bullets
	* 3884eab Add color
	* 3e42136 now using requestAnimationFrame
	* 4035769 frame interval was set wrong after game was paused
	* 25ede83 a couple missing ends with the ipad version
	* df03538 I can't spell 'screen' apparently :)
	| * 354dfdd Make ships able to spawn on coins
	| * 0c6daf1 Make it possible to collect coins
	| * a3c0ae4 Create helper functions
	| * 656b02e First pass at adding coins
	|/  
	* b0678b1 Revert controls
	
If you 'checkout' to a non-HEAD change, then edit a file and commit that change will not 
part of that branch and will be lost when you 'checkout' to HEAD or switch to another branch.

If you want to save the commit you need to create a new branch after you have commited this
unreachable change with this command;

`git checkout -b new_branch_name`

_How do the diagrams help you visualize the branch structure?_

Diagrams help me to understand the relationship between branches and understand which
changes are in which branches.

To merge branch 'coins' into branch 'master'

`git merge master coins`

To see what changes where made in a particular change number:

`git show <change_number>`

_What is the result of merging two branches together? Why do we represent it in the
diagram the way we do?_

The result is that all the changes made in the two branches are merged together into a 
single commit. We represent it that way because it shows that changes now have two sets of
parent commits.

_What are the pros and cons of Git's automatic merging vs. always doing merges manually?_

Gits automatic merge will reduce the work we have to do when merging branches. The problem
with automatic merges is that they may introduce design bugs as they are just doing a text
based analysis to know when merge. With manually doing merges a person can analyze the code
so that the merge maintains design intent of the code.
