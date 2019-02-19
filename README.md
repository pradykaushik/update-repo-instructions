# update-repo-instructions

## Create a new repository on github using the fork link under piazza#resources tab.
Under the resources tab in piazza, you should be able to find a link to Lab 3.
If you haven't clicked on it and created a repostory for lab2 and lab3 already, then you can just click one of the following links.
* [lab3](https://classroom.github.com/a/db52zvT7)
* [lab2](https://classroom.github.com/a/0jVQB1sr)

## Updating remote link.
1. Navigate to the GitHub landing page for the respective lab repository.
2. Click on the button that says _Clone or download_ and copy the link.
3. On your local machine, navigate to the directory that has your lab2/lab3 code (the one that you had earlier cloned into).
4. To make sure you're in the right directory,
	- type the command `git remote -v`. You should see links that contain _binghamtonuniversitycs-240_ in them.
5. Now, run the following commands to set a new remote link (the one you copied from the GitHub landing page) as upstream.
	- type the command `git remote set-url origin <new url>`. It might ask you for your password.
	- type the command `git remote -v`. You should now see links that contain _bucs240_ in them. If you don't see observe this change, please post on piazza.
6. Once you have updated the remote links, we need to perform a `git pull ...` once before moving to the next steps.
	- type the command `git pull origin master`. If it opens up an editor for you, just exit without making any changes.

## Pushing code to new repository.
By now you should have successfully updated the remote links. To push the code to the newly repository, follow the below steps.
* First commit any changes by running the following commands in sequence.
	- `git add --all`
	- `git commit -m "adding lab3 code to new repository."`
	- `git push origin master`

You should be all set now. Navigate to the GitHub page and you should see your code there.

**Good Luck!!**
