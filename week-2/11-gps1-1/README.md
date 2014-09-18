# GPS 1.1 Git work flow and branching

## Learning Competencies
- Establish a git work flow with a collaborator
- Explain what a git branch is and its purpose
- Demonstrate the ability to research for debugging or to better understand concepts


## Summary
<!-- Need summary here -->

## Releases

## Release 0: Fork the repo

Choose 1 member of your pair and fork [this repo](https://github.com/Devbootcamp/phase-0-gps-1). Add your guide and your pair as collaborators on your fork. Inside there is a file called file_1.md, file_2.md and file_3.md
<!-- Can we change the file names to step-1, step-2, and step-3? or name them after what they are doing in each step? -->

## Release 1: Clone the Repo
Both you and your pair should clone the newly-forked repo to your own computer.

## Release 2: Create a Feature Branch

Now the driver will create a feature branch called feature-1. Follow the instructions in file_1 and file_2. You will change file_3 in the next release. After you've made the changes, push your branch to GitHub and do a pull request to master. The navigator should review the pull request on GitHub and merge after a brief review.

Take some time to talk about why you would bother creating a feature branch in the first place. Make sure you could explain what a branch is, how to create one, and how to navigate between them.

## Release 3: Fetch and Merge

Switch driver and navigator roles, now the other partner will make modifications. But first the new driver will need to incorporate the changes already pushed to GitHub. Fetch and merge the changes to your local repository.

Make a new branch and follow the instructions for changing file_1 and file_3.

Make a pull request like last time. The navigator should review the request and merge it. You will be using this work flow all the time as a developer!

## Release 4: Merge Conflict
Sometimes you will encounter merge conflicts, but don't worry, once you've gone through a few, they aren't as scary, so it's good to get practice now!

A merge conflict happens when two branches change the same file and try to merge them together. Here is how to create a small merge conflict:

<!-- Who should do this? -->
1. Create a branch called small-conflict, make a change in file-1, add and commit.
2. Check out the master branch, in the same place that you made a change on small-conflict, make a different change. Add and commit this change.
3. Merge the small-conflict branch to the master.
4. Resolve the merge conflicts.

You can imagine that in a big project, this can be a huge time waster. Good git work flow can prevent merge conflicts from being a problem.


## Release 5: Discuss

Confer with your partner and guide about what a good git work flow is, the purpose of git branching, feature branching, and pull requests. You are in the elite programming group of git users now!

## Release 6: Reflect
On your own, reflect on this challenge in the [my_reflection.md](my_reflection.md) file.


