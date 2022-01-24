# Intermediate - Working with Branches

**Purpose**: Become familiar with the concepts of Branches and when to use them

**Task**: Learn about conventions when working with branches. Create 2 branch, switch to one, create a file, switch to second branch and change file

**Outcome**: Learning the concept of Branches and how to use them

## What are Branches?

Branches are a way to keep projects organized with different versions. For example, one branch is always "main" (or "master") and a second could be "board-developement". Then you can make changes on "board-development" withouth affecting other branches. Once the code works, you can push to main. "Main" should be the latest **working** version of everything. 

## Naming Conventions and Structures

If you are adding a feature to the code base start the branch name with "feature-[FeatureName]" where FeatureName is what you plan on adding. 

## Create a new branch

From the github desktop you can go to `Current Branch -> New Branch`

From the terminal you can say: 

    git branch [BranchName]

which will create a new branch, then you can switch to it. 

or **(recommended)**

    git switch -c [BranchName]

which will create and switch to the new branch.

To Switch between branches you can use `switch` or select the branch in the github desktop. 

## Create a Second Branch

Here's something you can try: In this repository, add a branch with your user name. Then create and add a file in the `data` folder that is called **bookRecommendation** and has the name of your favorite book. 

Start by going to the main branch and [creating a new branch](#create-a-new-branch). Then create a new text file and commit and push to that branch. Then you can switch back to main and see that the file does not exist in main. 

## Deleting a branch

This is possible, and very helpful for cleaning up a messy repo. However, in AERO, only leadership should be deleting branches. Create as many helpful branches as you need and be sure to follow good naming conventions to keep track of what changes are on that branch. Once you do your changes, be sure to incorporate them back to main (or another applicable branch). 

## Next Up

The next step is to merge changes from one branch to another one. See the [Next Tutorial](2_Merging_Information.md) to learn more about merging. 
