# Git Commands:

## Syncing Data

**Push:**
The Push command is used to publish and save the changes you made to your code to the remote repo (on Github). This command saves your changes and makes them available to everyone else who can see the repo. The command can be called like this: ```git push``` while inside the branch you would like to push to. <br />

**Pull:**
The Pull command is used to bring any changes that might have been made to the repo down to your local copy. So if somebody modified the code and pushed, you would then use Pull to bring the new code to your computer for you to edit and view. The command be called like this ```git pull``` while inside the branch you would like to pull from. <br />

**Add:**
The Add command allows you to stage your changes, you're pretty much gathering all the files you would like to Commit and Push. So it would be called like this ```git add file1 file2 etc```. After and only after using the Add command can you Commit and Push.

**Commit:**
The Commit is a lot like the save button for your code. It functions in a similar manner to that of the Push command, but instead of how Push updates the repo in remote storage (on Github), the Commit command simply saves your work and doesn't make your changes available to others. So this is very helpful if you want to have your code saved locally and on the in a remote place interent, but it's not ready for implementation yet. The command can be called like this ``` git commit``` or preferably ```git commit -m "commit mesage/description"```<br />

**Clone:**
The Clone command allows you to bring a complete copy of a codebase to your local folder, so if you don't already have the code on your computer, then you can use the Clone command to bring it down to for local use. ```git clone "link to repo here"```<br />

**Fetch:**
The Fetch command is a like like the pull command, except it brings only other people's commits down to your local branch, unlike the Pull command which brings down all Pushes to your local branch. The command can called like this ```git fetch``` while inside the branch you would like to fetch from. <br />

## Merging Changes

**Merge:**
The Merge command allows you to apply the changes you made to code from one branch to another, it's kind of like a highway on-ramp, all of the previous code is still on the highway, you're just adding new code to what already exists. The command can be called like this ```git merge``` while inside the branch you would like to merge to. <br />

**Checkout:**
The Checkout command allows you to change your current working branch on Github. This command also allows you to create a new branch and then get to working inside of it right away. The command can be called like this ```git checkout``` while inside the branch you would like to checkout.<br />


## A Helpful Diagram
<p align="center">
  <img src="images/git-commands.png" />
</p>

## Even More Documentation on Git:
Believe it or not, this is pretty much scratching the suface of the full range of functionalilty that Github offers, so [here](https://docs.github.com/en) you can do futher reading if you'd like to learn even more about the wonderful world of Github!


## Example of Multiple Commands:
```git clone "https://github.com/uvmaero/AERO_Tutorial"``` <br />
~ make some changes to the code  & while inside the working folder in your terminal~ <br />
```git add fileThatWasChanged``` <br />
``` git commit``` <br />
```git push```<br />
now any changes you made are saved and pushed to the uvmaero/AERO_Tutorial repo!<br />


If you have any questions at all, please reach out!!! George and I are more than willing to help answer any questions!!!!




