[Week 1 Home](../)

# Tracking Changes

## Learning Competencies

- Explain the process from creating a change to a commit.
- Demonstrate best practices for commit messages
- Explain the 3 states of a file in git (working, staged, commit)


## Summary


## Releases

## Release 1: What is a change?

Here is the video that goes along with this concept:

[Tracking Changes](https://www.youtube.com/watch?v=cBTs3WWMXUs)

Git works by following all of the changes in the files inside a git tracked folder. The save point in git is called a commit. Think of a commit like a checkpoint in a video game. It is a point where you can go back to and look at the state of the files at that commit. Just like in a video game if you die to a boss or make the wrong decision, you can go back to the checkpoint. This saves the pain of starting over from the beginning. A commit is your safety net if you accidentally introduce bugs in your code. You can revert to a working state while you debug your code. It is a great idea to commit often to create more frequent save points to fall back on.

For this reason, it is important to start getting in the habit of writing good commit messages. Here is the style guide for commits [Tim Pope's style guide](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html). Note that there is a bunch of advanced git talk here, just focus on the first part of the post. Note that you can type your commit your messages in your terminal with `git commit -m "message goes here between the quotes"` or you can use the verbose commit message to give yourself some room `git commit -v` will open your default editor according to git (learn how to change it [here](https://help.github.com/articles/associating-text-editors-with-git) follow instructions for sublime). After you write your message, save and close the file. Your commit will be recorded.

Check the curriculum commit history by typing `git log` and scroll using the up and down arrows. Exit using q. How would you score our git commit messages? Would you know where to look in each message to find what files were changed?

Whenever you change the state of a file, say from blank to with some letters on it, adding or deleting a file, it is tracked. You can check the status of all the files in the local repo by typing `git status` . If you have modified any files you will see some categories: Changes not staged for commit:, Changes to be committed:, and if you have created a new file, Untracked files:. No changes would return the message:

`On branch master
nothing to commit, working directory clean`

You can only push changes that have been committed.

Git also gives you handy instructions below these categories. In untracked files it tells you how to add the files (use "git add <file>..." to include in what will be committed) from untracked to staged(changes to be committed), and how to remove a file from the added section to bring it back to untracked (use "git reset HEAD <file>..." to unstage).

If you commit some files and decide that you actually want to change the files, use the command

`git reset --soft HEAD^`

HEAD is the commit you are currently on, HEAD^ is the last commit, HEAD~3, HEAD~4, HEAD~5, are the 3rd 4th and 5th commit from HEAD respectively.


## Release 0

So now we know about how to track changes, lets make some!

- write something in my_reflection.md
- check your git status
- write something in this README.md
- check your git status (notice a pattern?)
- add the change for my_reflection.md
- unstage the change for my_reflection.md
- add and commit the changes for my_reflection.md
- check the git log to see your commit and message
- reset the last commit

## Reflection

Now that you are an expert on git changes, include a brief summary of how we can use the power of git tracking to make our lives as developers easier. Answer the questions on the my_reflection.md.

Make sure you make a great commit message when done with this challenge.