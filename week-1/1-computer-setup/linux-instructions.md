[Week 1 Home](../)

# Computer Set-Up Instructions - Linux

## Learning Competencies
- Install technologies from the command line
- Use package managment tools


## Summary
You will need to have your computer set up with the following tools for Phase 0 of Dev Bootcamp. Make sure to go through this guide step-by-step. You'll need to have each of these technologies installed to have a smooth start to Phase 0 and your future career!

## Releases
(i.e. directions - each release is necessary for the next release, so be sure to do everything in the order specified for all challenges)

## Release 0: Download Sublime Text 2
Download and follow instructions from [their site](http://www.sublimetext.com).

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
Now we are ready to install RVM

## Release 3: get RVM

RVM will take be our ruby version manager. Gems will install here and we will use its copies of Ruby over our system Ruby. Yay!

```shell
\curl -L https://get.rvm.io | bash -s stable --ruby
```

this installs RVM and also installs the latest stable version of Ruby.


## Release 4: Set up your Path
First you need to clone this github repository into your computer and install the files. Type each line separately:

```shell
git clone https://github.com/supertopher/dotfiles.git
cd dotfiles
./install
```
Installing these files will configure your bash profile, enable autocomplete, always display rspec with color, and allow you to use "subl" as a shortcut to open sublime.

Restart your terminal to have these changes take place.

Note: These dotfiles should run fine with Linux, but some commands may not execute. The Sublimelink command will not work.

## Release 5: Install Git

We will use apt-get to install git:

```shell
sudo apt-get install git-core
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

## Release 7: Install Node
Node allows you to run Javascript in your terminal.

```shell
sudo apt-get install nodejs
```

You'll use this later in Phase 0.

## Release 11: Install Rspec
Type ```gem install rspec```

This will install RSpec, a ruby testing framework.

## Release 12: Install SQLite
<!-- check for use with Rbenv -->
RVM installed SQLite3 for us, make sure by typing

```shell
sqlite3 --version
```
This should return your current version. If it does you should be all set!

## Release 13: Install Postgres
Type the following commands one at a time:

```shell
sudo apt-get install postgresql
```

follow the instructions during the install and you will be set. Check your install by typing:

```shell
psql -V
```
make sure its a capital V, this prints the version and exits. If you get into psql command line hit CTRL + D to exit.

## Thats all

You now have a set up environment for development! If you are interested in this kind of thing, there is a whole job created around automating server and terminal set up. It is called DevOps, they do lots of things to make software development more efficient. Check it out! [devopsreactions](http://devopsreactions.tumblr.com/)
