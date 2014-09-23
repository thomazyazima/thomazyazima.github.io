[Week 1 Home](../)

# Computer Set-Up Instructions - Linux

## Learning Competencies
By the end of this lesson, you should be able to:
- Install technologies from the command line
- Use package managment tools


## Summary
You will need to have your computer set up with the following tools for Phase 0 of Dev Bootcamp. Make sure to go through this guide step-by-step. You'll need to have each of these technologies installed to have a smooth start to Phase 0 and your future career!

## Releases
(i.e. directions - each release is necessary for the next release, so be sure to do everything in the order specified for all challenges)

## Release 0: Download Sublime Text 2
Download and follow instructions from [their site](http://www.sublimetext.com).

After you download, create a symlink so you can open sublime using `subl "filename"`

Enter this command in to you terminal:
```shell
sudo ln -s /opt/SublimeText2/sublime_text /usr/bin/subl
```

test by typing subl . it should open all files in your current directory!

You don't have to purchase your license right away, you can "cancel" out of the dialog box as many times as you would like, but it is good practice to buy a license after you decide you like it. (Since eventually you're hoping to get paid for writing programs, you want to pay it forward in advance.)

## Release 1: Your Operating System
These instructions are optimized for use with Ubuntu. If you are using a different version of Linux you may have to translate as needed to your particular OS.


## Release 2: Get ready for install

First step is to update our package manager apt-get. This will be done using this command:

```shell
sudo apt-get update
```

If that went without error you can now get curl:

```shell
sudo apt-get curl
```
Now we are ready to install Rbenv

## Release 3: get Rbenv

Rbenv will be our ruby version manager. Gems will install here and we will use its copies of Ruby over our system Ruby. Yay!

Digital ocean wrote a great how-to on getting Rbenv and Ruby running on Ubuntu. Follow the instructions here. This will also handle installing nodejs. Make sure that you install ruby 2.0.0-p353 instead of 1.9.3-p392.

Also the step to open the .bashrc and fix the path is done in Release 4 so no need to complete those steps during this release

[Digital Ocean](https://www.digitalocean.com/community/tutorials/how-to-install-ruby-on-rails-on-ubuntu-12-04-lts-with-rbenv--2)

## Release 4: Set up your Path
First you need to clone this github repository into your computer and install the files. Type each line separately:

```shell
git clone https://github.com/supertopher/dotfiles.git
cd dotfiles
./install
```
Installing these files will configure your bash profile, enable autocomplete, always display rspec with color, and allow you to use "subl" as a shortcut to open sublime. Note: this will replace your current bash profile. 

Restart your terminal to have these changes take place.


## Release 5: Install Git

This should have been installed if you followed the digital ocean tutorial in release 3. Check by typing:

```shell
git --version
```

## Release 6: Configure Git
You then need to overwrite .gitconfig to your own username and password in GitHub. Use your name and your Github email address in the following format:

```shell
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

Now make sublime text your preferred editor for git:
```shell
git config --global core.editor subl
```

## Release 7: Set up Sublime
Follow [these instructions](https://github.com/Devbootcamp/phase-0-handbook/blob/master/text-editor-setup.md) in the Phase 0 Handbook to make Sublime your default text editor.

## Release 8: Install Node
Node allows you to run Javascript in your terminal.

You should have installed this when installing Rbenv if yo used the digital ocean guide.

Test by typing:

```shell
node -v
```

You'll use this later in Phase 0.

## Release 9: Install Rspec
Type ```gem install rspec```

This will install RSpec, a ruby testing framework.

## Release 10: Install SQLite
Install sqlite3 using apt-get

```shell
sudo apt-get install sqlite3 libsqlite3-dev

gem install sqlite3-ruby
```
type sqlite3 -version to test.

## Release 11: Install Postgres
Type the following commands one at a time:

NOTE: If you have trouble installing postgres, don't worry about it. You won't need it until Phase 2. We wanted to have it set up in advance when your path was all sqeakly clean and wonderful, but if you have trouble, just move on.

```shell
sudo apt-get install postgresql
```

follow the instructions during the install and you will be set. Check your install by typing:

```shell
psql -V
```
make sure it's a capital V, this prints the version and exits. If you get into psql command line hit CTRL + D to exit.

## Thats all

You now have a set up environment for development! If you are interested in this kind of thing, there is a whole job created around automating server and terminal set up. It is called DevOps, they do lots of things to make software development more efficient. Check it out! [devopsreactions](http://devopsreactions.tumblr.com/)
