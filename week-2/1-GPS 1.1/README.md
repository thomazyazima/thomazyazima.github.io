# GPS 1.1 Git work flow and branching

## Objectives
- Establish a git work flow with a collaborator
- Explain what a git branch is and their purpose
- Use research methods to learn more about languages

## Release 0

Choose 1 member of your pair and fork the git repo called phase-0-gps-1. Add your guide and your pair as collaborators on your fork of [this repo](https://github.com/Devbootcamp/phase-0-gps-1). Inside there is a file called file_1.md, file_2.md and file_3.md

## Release 1

Clone:

Both you and your pair should clone the newly forked repo to your own computer.

## Release 2

 Now we are going to create a feature branch called feature-1. Follow the change instructions in file_1 and file_2. We will be changing file_3 in the next release. When you finish your changes, push your branch to github and do a pull request to master. Review the pull request on github and merge when you are ready.

Take some time to talk about why you would bother creating a feature branch in the first place. Make sure you could explain what a branch is, how to create one, and how to navigate between them.

## Release 3

Switch driver and navigator roles, now the other partner is going to make some modifications. First you are going to have to incorporate the changes your pair pushed to github. Fetch and merge the changes to your desktop.

Make a new branch and follow the instructions for changing file_1 and file_3.

Make a pull request like last time, review the request and merge them. You will be using this work flow all the time as a developer!

## Release 4

 Now we are going to create a merge conflict. A merge conflict happens when a commit happens after you branch, and the same file is modified in both branches. Here is how we can create a small merge conflict on the desktop:

 1. create a branch called small-conflict, make a change in file-1, add and commit.
 2. Check out the master branch, in the same place that you made a change on small-conflict, make a different change. Add and commit this change.
 3. Merge the small-conflict branch to the master.
 4. Resolve the merge conflicts.

 You can imagine that in a big project, this can be a huge time waster. Good git work flow can prevent merge conflicts from being a problem.


 ##Release 5

Confer with your partner and guide about what a good git work flow is, the purpose of git branching, feature branching, and pull requests. You are in the elite programming group of git users now!




