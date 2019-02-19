# update-repo-instructions

## Lab2 and Lab3 update
### Create a new repository on github using the fork link under the [piazza#resources](https://piazza.com/binghamton/spring2019/cs240b1/resources) tab.
Under the resources tab in piazza, you should be able to find a link to Lab 2 and Lab 3.
If you haven't clicked on it and created a repostory for lab2 and lab3 already, then you can just click one of the following links.
* [lab3](https://classroom.github.com/a/db52zvT7)
* [lab2](https://classroom.github.com/a/0jVQB1sr)

### Updating remote link.
1. Navigate to the GitHub landing page for the respective lab repository.
2. Click on the button that says _Clone or download_ and copy the link.
3. On your local machine, navigate to the directory that has your lab2/lab3 code (the one that you had earlier cloned into).
4. To make sure you're in the right directory,
	- type the command `git remote -v`. You should see links that contain _binghamtonuniversitycs-240_ in them.
5. Now, run the following commands to set a new remote link (the one you copied from the GitHub landing page) as origin.
	- type the command `git remote set-url origin <new url>`. It might ask you for your password.
	- type the command `git remote -v`. You should now see links that contain _bucs240_ in them. If you don't see observe this change, please post on piazza.
6. Once you have updated the remote links, we need to perform a `git pull ...` once before moving to the next steps.
	- type the command `git pull origin master`. If it opens up an editor for you, just exit without making any changes.

### Pushing code to new repository.
By now you should have successfully updated the remote links. To push the code to the newly repository, follow the below steps.
* First commit any changes by running the following commands in sequence.
	- `git add --all`
	- `git commit -m "adding <lab2 or lab3> code to new repository."`
	- `git push origin master`

You should be all set now. Navigate to the GitHub page and you should see your code there.

## Program 1 update
Last week each of you individually forked [program1-template](https://github.com/bucs240/program1-template) repository, added your partner as a collaborator started working on program1.
Once you have created a team GitHub, you should have a repository created for you for program1.

To push current code for program1 to the new repository, follow the below steps.
Let's say that the directory you were earlier working in is called _old-dir_.
1. Create a separate directory called _program1_.
2. Change working directory to _program1_ using the command `cd program1`.
3. Clone the new repository using the available by clicking on the _Clone or download_ button on the GitHub landing page. This would create a directory called _program-1-spr19-<team>_.
4. Change working directory to _program-1-spr19-<team>_ using the command `cd program-1-spr19`.
5. Copy over all the files from _old-dir_ (except driver code and README.md) over to current directory.
6. Use the below commands to add, commit and push code to the new repository for program1.
	- `git add --all`
	- `git commit -m "added all source files from old repository."`
	- `git push origin master`

You should be all set now. Make sure that both you and your partner have cloned from new repository by checking that the result of `git remote -v` for you and your partner is the same.

**Good Luck!!**
