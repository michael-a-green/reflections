#Lession 1 Reflections

*How did viewing a diff between two versions of a file help you see the bug that was introduced?*

It pin pointed the changes that were made between the two files. So then all I needed to do was 
examine the change to see if it was done correctly.

*How could having easy access to the entire history of a file make you a more efficient
programmer in the long term?*

Having easy access to the history of the changes of the program enables me to identify
what could possibly be contributing to whatever I'm observing in the current version and
allows met to go back in time (one change at a time) to examine how each change affecting
the functionality of the program.

*What do you think are the pros and cons of manually choosing when to create a commit,
like you do in Git, vs having versions automatically saved, like Google Docs does?*


Pro:

When you commit based on your own decision-making, you can create check points based on
a logical development plan. Each change can be a functional representation of a feature.

Con:
If you don't go through and carefully plan your development before you start coding, then
your commits may be jumbled and difficult to understand from one change to another. In this
case automatically saving would at least increase the chance of capturing a logical
progression of development.

*Why do you think some version control systems, like Git, allow saving multiple files in
one commit, while others, like Google Docs, treat each file separately?*

It's because Git is geared to software developers. A single software feature can span
multiple files and so oftentimes changes to multiple files need to be on the same change number
so that they can be grouped together into a single logical update.

*How can you use the commands git log and git diff to view the history of files?*

You can use `git log` to see the history of all changes in a repository. It lists each change
along with a unique ID# for the change and a description of what was changed.
You can then use `git diff` to see specifically what changes were made between two
different changes.

*How might using version control make you more confident to make changes that could break something?*

I'm more confident because with version control any change I make that causes a bug can 
be identified and then backed-out by 'git checkout' and 'git diff'

*Now that you have your workspace set up, what do you want to try using Git for?*

To tell what version my workspace has checked out and whether I have any changes in my 
workspace that may need to be submitted.


