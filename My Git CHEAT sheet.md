#						My Git CHEAT sheet
-------------------------------------------------------------------
Command 					|	Usages 
-------------------------------------------------------------------
git status	                |	Shows the status of the git repo 
 							|	that how many files are committed 
 							|	or not
-------------------------------------------------------------------
git init					|	Initialize the repo
-------------------------------------------------------------------
git log						|	Shows the commit history
-------------------------------------------------------------------
git add .					|	To add all changes
-------------------------------------------------------------------
git add (file name) or 		|	Tell git  to track the changes
(with location file name)	|
-------------------------------------------------------------------
git commit –m"message"		|	Add changes to the original repo 
							|	and tag a message
-------------------------------------------------------------------
git push origin "branchname"|	To push the changes successfully 
 							|	to “branchname”.
-------------------------------------------------------------------
git pull origin "branchname"|	To pull the changes successfully 
 							|	to “branchname”.
 							|	or even to bring a new branch.
-------------------------------------------------------------------
git checkout				|	Shows on which branch you are.
-------------------------------------------------------------------
git checkout branchname		|	To switch to “branchname”
-------------------------------------------------------------------
git branch 					|	List all brach names
-------------------------------------------------------------------
git branch -d <branch name>	|	Delete the branch(make sure to move 
							|	to other branch before deleting as
							|	it is obious)
-------------------------------------------------------------------
git branch -D <branch name> |	Delete the branch even having some
							|	commits not push to origin.
-------------------------------------------------------------------
-------------------------------------------------------------------
##		Rebaseing a forked repo with git rebase
-------------------------------------------------------------------
Step 1: Add the remote (original repo that you forked) and call it “upstream”

	[git remote add upstream originalrepo address]


Step 2: Fetch all branches of remote upstream

	[git fetch upstream]


Step 3: Rewrite your master with upstream’s master using git rebase.

	[git rebase upstream/master]


Step 4: Push your updates to master. You may need to force the push with “--force”.

	[git push origin master --force]

-------------------------------------------------------------------
##		push a local initialized repo on github

		1.) git init.
		2.) git add .
		3.) git commit -m "first commit"
		4.) git remote add origin "remote repository URL"
		5.) git push origin master.


-------------------------------------------------------------------
Making new branch localy and hen publishing it on remote.
	1.) git checkout -b <branch name>
 	2.) git push --set-upstream origin responsive

-------------------------------------------------------------------


		