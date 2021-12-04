# Getting Start With Git Using GitHub Desktop

**Purpose**: Become familiar with Git commands in the GitHub Desktop

**Task**: Clone a repository, modify a file, add and push changes

**Outcome**: Understanding how to use git to get files and publish changes

## Getting the client

You can use the [GitHub Desktop](https://desktop.github.com/) client to pull and push changes (among many other features). Once you have it, sign in and clone this repository. 

Once downloaded, follow the onscreen instructions to setup the client. One option that you'll want to change is the default editor. Go to `File > Options ` to make changes. (psst. I recommend [VSCode](https://code.visualstudio.com/))

## Cloning the repository (repo)

In GitHub Desktop, go `File > Clone Repository`. Then use the filter to find "AERO Tutorial". Then press `Clone`. Now click on `Show in Explorer` to open up the containing folder. 

## Making a change to a file

Now that you have this folder downloaded, it's just a folder on your computer. You can do pretty much anything you want to it. So, let's change a file. In the explorer (in the repo you just download) go to `data` folder. Open the `favorite-animal.txt` file and add your favorite animal at the end of the file. Save your changes. 

## Commit Changes

Go back to GitHub Desktop. In the AERO Tutorial repo, you should see that one file change. It should show the changes if you click on that file. To commit the changes, select which files to commit (should only have the one right now) and type a commit message. 

The commit message is in the bottom left. It will have a default message for you. Click in the first box and type a brief message. Commit message are an art. They should be descriptive and short. For this, type `adding another animal`. The 'Description' area is for longer messages. Dont' worry about that yet. 

Now press `Commit to main`. 

## Push Changes

Good, now the changes are saved, but they are not available to everyone else. To solve that, look at the top bar, there should be an option to "Push Origin". Do that. If everything went well, you should have a screen that says "No Local Changes". (FYI: local means 'on your machine' whereas remote is what's published everywhere else)

## WARNING: MERGE CONFLICTS 

Merge conflicts are what happens when two of the same files were committed to the branch with conflicting information. 

For example, let's say John and Sarah are working on `favorite-animals.txt` at the same time and John changes line 4 to say "Dog" while Sarah changes line 4 to say "Cat". Both can commit the file in the way you just did. If Sarah tries to push the changes, they can. Now when John tries to push the changes, their local repository is actually old and the push won't work since John's change to the file would conflict with Sarah's. 

If this happens to you, GitHub Desktop will prompt you to open the conflict in VSCode (or another default editor). Go to that editor to accept or decline the changes. See [VSCode Tutorial](1_VSCode_GettingStarted.md) for a section on dealing with Merge conflicts. These can get very confusing even for long time Git users. So, if you get stuck at this step, don't fret! Reach out for help. 

## Verify Changes

GitHub only shows the remote version of the repo. So, if you want to check if your changes actually pushed or not, you can go to the [AERO Tutorial](https://github.com/uvmaero/AERO_Tutorial) GitHub repository and check what that version says. If it's different than you expect, double check you "push orgin" after commiting. 