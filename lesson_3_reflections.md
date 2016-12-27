#Lession 3 Reflections


* create an empty repo on GitHub
* git repositories on GitHub: "remotes"

Push data: Send data to a "remote."



To view remotes:

`git remote`

To add a repository to the remote

`git remote add <remote_name> <github_url>`

Full examples:

(uses SSH address)
`git remote add origin git@github.com:cbuckey-uda/reflections`

(uses HTTPS)
`git remote add origin https://github.com/michael-a-green/reflections.git`


_When would you want to use a remote repository rather than keeping all your work local?_

If you want to protect your code and the changes to your code from loss, it's good to have
an online backup. In this case you get it for free.

Having a remote repository enables you to more easily collaborate with others (get people 
to help you develop, document, or verify your code). You don't have to setup your own 
repo server GitHub has done that for you.

If you want to publish something to a wide audience you can do so with GitHub. That way 
you don't have to figure out how to do it yourself.

