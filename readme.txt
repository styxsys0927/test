This is a tutorial of how to use Git.

1. Download Git and launch git bash
2. Create an account:
	$ git config --global user.name "username"
	$ git config --global user.email "useremail"
3. Create a work directory
	$ mkdir test
	$ cd test
	$ pwd (check path)
4. Init git project
	$ git init
5. Add file
	$ git add readme.txt
	$ git commit -m "A readme of how to use Git"
6. Check status changes
	$ git status
	$ git diff
7. reset status
	$ git log
	$ git reset --hard HEAD^ (the last version; HEAD^^: two versions before; HEAD-100: 100 versions before)
	$ git reset --hard <partial commit id> (can be used to reverse rollbacks)
	$ git reflog (check former allocated commit ids)
	
8. create a new repository on github and push the local one
	$ git remote add origin git@github.com:styxsys0927/test.git
	$ git push -u(only for the first time) origin master
9. clone remote repository to local one
	$ git clone git@github.com:styxsys0927/test.git
10. use branch
	$ git checkout -b dev (create branch)
	$ git branch dev
	$ git checkout dev (swich to branch)
	$ git checkout master
	$ git merge dev
	$ git branch -d dev (delete branch)
	