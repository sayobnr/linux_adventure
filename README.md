welcome to my Linux adventure
How to fix git error: There is no tracking Information for the current branch.
Note: When performing an operating like git pull, git push, git fetch etc, WITHOUT SPECIFYING THE REOTE OR THE BRANCH INVOLVED IN THE OPERATION, you should first make sure that the current branch has a corresponding upstream.

Depending on how the push.default congig is set, you may encounter the error above.

to solve it, you have to push or pull with the complete url address of the repo's github and the name of the local branch you are pulling or pushing through:

git pull/push/fetch https://github.com/sayobnr/linux_adventure.git main 
press enter and it will ask for your git username. After providing your git username, you will be rasked to provide your password, but what you need is your access code. Note that when your try to type, there will be no disply on yor screen, but it's really typing. This is a security measure github employed to protect your password/access code. Therefore, to fill in your password, you just need to copy and paste and click enter and your upstream will be established.

Alao note that you can get the name of your branch with the command 'git branch'
yuo can get your remote repo name and url with 'git remote -v.
