[Week 1](README.md)

# Computer Setup (Mac Users)

## Learning Competencies


## Summary
If you have a mac computer, you'll benefit from our learning (or bias) towards unix operating systems. Our San Francisco computer set-up expert has been kind enough to create these "dotfiles" which will make your environment mirror the Dev Bootcamp computers and fix a lot of path issues.

Note: You'll need either RVM or Rbenv installed to run these files. This will not install ruby.


## Releases

## Release 0: Clone the dotfiles
Navigate to [Topher's Dotfiles](https://github.com/supertopher/dotfiles)

**BEFORE cloning, always make sure you check your repository. You don't want to clone repositories into other repositories -- you'll get yourself into a load of hurt, so do a nice `pwd` in the command line and navigate to the directory you want to clone to.**

Using your git knowledge, clone this repository onto your computer. There is no need to create a branch unless you intend to contribute or propose a change to his files.

## Release 1: Run the Scripts
Using your terminal, navigate to the dotfiles repository. Once you are in there, you'll want to run:

```shell
./install

```

If you get a weird message about sublime, you can ignore it. 

If you want to create a symlink for Sublime Text 2 and 3, run:

```shell
./sublimelink
```

## Release 2: Re-configure GitHub
This standard install overwrites your github username and email. Make sure to reset them by typing (with your information):

```shell
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

## Release 3: You're computer should now be set up with some handy shortcuts. For example, you can now navigate to a directory in your terminal and type `subl .` to open all the files in that directory. Pretty neat, huh?





