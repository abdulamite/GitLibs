
# GitLibs
The purpose of this repository is to go over the basics of git and GitHub in a fun and easy way. In the exercise you will be forking this repository to your Github account, cloning your fork to your local machine, making some changes to a local file, and pushing back to your fork. Finally you will be creating a pull request to the master branch you forked in an attempt to merge your changes into the production codebase.

## Prerequisites
The tutorial assumes that you have a basic understanding of the command line and you have git installed on your local machine. If you do not have git installed on your machine, you can download the latest version below:
[https://git-scm.com/downloads](https://git-scm.com/downloads)

It is also important that we understand the difference between git and and Github. 

## git
git is an open source distributed version control system. git allows you to set up working directories and track changes in the files in the directory. This allows you to develop locally, create branches, log and revert project changes. It is perfectly reasonable to use git without the use of Github.

## GitHub
Github is an online hosting service for git repos. This allows you to build and collaborate on projects together. This makes it easy for companies, and open source groups to fork repos, create local copies of the application, and submit pull requests to the master copy. Essentially you will be able to take the code locally on your machine, and request to have it merged into the production version of the code.

## Getting Started
Now that we understand what we are doing and what we need, now we can finally get started!!

 1. First you will need to fork this repository so that we have this
    available on your Github account. To do this, simply click the fork
    button at the top right of the screen.
    
    <img src="https://upload.wikimedia.org/wikipedia/commons/3/38/GitHub_Fork_Button.png" width="18%">
    
	After forking the repository you should now have the repository available on your Github account.    
 2. You will now need to clone the repository you created. You can do this by going to the newly created repository available at [https://github.com/{your_github_username}/gitlibs](https://github.com/{your_github_username}/gitlibs)
**Please note that the above URL will fail because is not valid and you will need to substitute in your Github username**
 3. You can now clone the repository to your local machine by opening your terminal, navigating to an appropriate folder,  and running the following command substituting in your Github username: 
`git clone https://github.com/{your_github_username}/GitLibs.git`
 4. Now if you run `ls -l` you should now see the `GitLibs` directory is now available.
 5. You can now go into the directory by running `cd GitLibs` . 
 6. Now what we need to do is create a new branch. We need to work on a separate branch as we should never complete new features on our master branch and it is easier for us to track and revert file changes while on a separate branch. 
To create a new branch run `git branch lib_edit`. This will create a new branch for us called  `lib_edit`. 
 7. Now that we created the new branch, we need to checkout the new branch. To checkout the new branch simply run `git checkout lib_edit`.
 8. If we ever need to check what branch we are currently on, we can simply run `git branch` and we will see a `*` next to the active branch.
 9. Now you can run `ls -l`  to see the the folders available in the project. You should see a file titled `libs.txt`
 10. Using either nano or your favorite text editor your can now open this file to edit it. To open the file using the default editor on your machine simply run `open libs.txt`
 11. You should see there are spaces available where you can edit the file. Simply complete the Mad Libs like file to create your own fun story.
 12. Once you have completed this, save your file and run `git status` to view the changes made in project.
 13.  Now you are ready ready to stage your commits. To add the files to your staging area run `git add lib_edit`
 14. Now that the file has been staged, we can check the status of the file by running `git status`. This will show us the status of the staged, and modified files.
 15. We can now commit our changes. It is important that we add a useful commit message so the reviewer knows what to look for in the file changes. To commit the file run `git commit -m "filled in lib.txt file"`
 16. Finally we can push our changes up to our Github repository. To do this we run `git push https://github.com/{your_username}/GitLibs.git lib_edit`. 
**Note that when we run this, we are only pushing the changes to our Github fork of the original repository. We must now open a pull request to request to add our changes to the production copy of the code**

## Pull Request

 1. Now that we are done making changes to the file and we have pushed them up to our Github repository, we are ready to open a new pull request. A pull request is a request to add the changes you made to the code, to the maintainers codebase. 
 2. To open a new pull request, simply navigate back to your Github fork of the repository you cloned. You can access this at [https://github.com/{your_github_username}/gitlibs](https://github.com/{your_github_username}/gitlibs)
 3. You should now see a yellow banner on this page with the new feature branch you created, and a button that says `Compare & pull request`.
 4. Click the button, and now we will be taken to a screen where we can add some notes about the changes we made to the project. 
 5. It is important that we take some time to write a helpful comment so that the maintainer of the project knows what changes we made, and what the maintainer can do to test our changes.
 6. For now, we can just comment, `Completed libs.txt worksheet`
 7. Now we can click `Create Pull Request`.
 8. And thats it! 

You have now successfully copied another programmers project, made some changes to the project, and submitted a pull request to the project. At this point we can wait for the reviewer to look over the changes you made and the reviewer will either accept the changes into their repository, or will request that you make some edits before moving forward with this change. That's all for today, though I hope that this was helpful in you better understand how git and Github works. Please feel free to sumbit a Pull reques to improve the quality of this documentation!
