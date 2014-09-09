[Week 1 Home](../)

# U1.W1: Git Remote and Merge

## Learning Competencies

- Explain what a remote is
- Demonstrate knowledge by setting up remotes for origin and upstream


## Summary

Git uses remote URLs to figure out where to go on the Internet to push and pull files. You are basically telling git exactly where to go when you want to save your work, get your work to your computer, or fetch changes from the repo you forked from.


## Release 0

Watch this video about setting up your remotes.

[Remotes, fetching and merging](https://www.youtube.com/watch?v=5IIPWznBvok)

What do your remotes look like? use `git remote -v` to check the URLs if your remotes.

## Release 1

Add the devbootcamp repo as your upstream. It should look like this when you are finished.

origin  https://github.com/<USERNAME>/phase-0-unit-1.git (fetch)
origin  https://github.com/<USERNAME>/phase-0-unit-1.git (push)
upstream  https://github.com/Devbootcamp/phase-0-unit-1.git (fetch)
upstream  https://github.com/Devbootcamp/phase-0-unit-1.git (push)

<USERNAME> should be your own user name.


## Release 2

When your new week is released, come back to this challenge and follow the video instructions on fetching and merging from devbootcamp's repo.

If Maria specifies fetching from a specific branch, make sure to note that with your fetch and merge commands.

git fetch upstream <BRANCH>

git merge upstream/<BRANCH>

If you run into a merge conflict, use this video to guide you through fixing the issue.

[Merge Conflict](https://www.youtube.com/watch?v=NW9AVnzx1B8)

## Reflection

Give a brief summary of what the purpose of a remote is and how to set it up. What are some other commands you can use to manipulate your remote? (use git remote --help to open the git docs)