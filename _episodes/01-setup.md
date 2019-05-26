---
layout: episode
title: Installation, configuration and accounts
teaching: 30
exercises: 0
questions:
  - How do I set up and configure Git on my laptop?
objectives:
  - Prepare your laptop for a CodeRefinery workshop.
---

# Git and GitHub preparations

To get started with Git and catch up with the basics, you need to install and configure 
Git, set up a GitHub account and set up a text editor to use with Git. 

This overview shows you how to:
- Set up a GitHub account
- Set up SSH keys
- Install Git
- Configure Git
- Set up a text editor

## Setting up a GitHub account

You will need an account at [GitHub](https://github.com) for parts of the CodeRefinery
Git lessons. Basic GitHub accounts are free. 
We recommend you to create a GitHub
account if you don't have one already. Please consider what personal
information you'd like to reveal. For example, you may want to review [these
instructions](https://help.github.com/articles/keeping-your-email-address-private/)
for keeping your email address private provided at GitHub.
Instructions for removing GitHub accounts 
[can be found here](https://coderefinery.github.io/installation/#instructions-for-removing-accounts).

## Setting up SSH keys

Using the SSH protocol, you can connect and authenticate to remote servers and
services. With SSH keys, you can connect to GitHub without supplying your
username or password at each visit.

Follow [this guide](https://help.github.com/articles/connecting-to-github-with-ssh/) to connect
to GitHub with SSH keys.

## Installing Git

To get started with Git, you need to make sure that Git is installed on your laptop
and that you have configured it correctly. Instructions for different operating systems 
are given below.  
Please follow the instructions but do not forget to also
[configure Git](#configuring-git).

### Installation on Linux

If Git is not already available on your machine you can try to install it via
your distribution package manager. Step-by-step instructions are provided in the
[installation instructions](https://coderefinery.github.io/installation/git/#installation-on-linux).

Please also verify your installation, according to 
[these instructions](https://coderefinery.github.io/installation/git/#how-to-verify-the-installation).

### Installation on macOS

The installation of Git on macOS will depend on the version of your OS. 
An installation guide can be found in the 
[installation instructions](https://coderefinery.github.io/installation/git/#installation-on-macos).

Please also verify your installation, according to 
[these instructions](https://coderefinery.github.io/installation/git/#how-to-verify-the-installation).

### Installation on Windows

Git should be installed on your computer as part of the Bash installation, which is 
described in detail in these 
[installation instructions](https://coderefinery.github.io/installation/bash/#installation-on-windows).	

Please also verify your installation, according to 
[these instructions](https://coderefinery.github.io/installation/git/#how-to-verify-the-installation).

## Configuring Git

After signing up for a GitHub account and installing Git on your machine,
you should go through the following steps to configure Git.
First, the following commands will set your user name and email address:

```shell
$ git config --global user.name "Your Name"
$ git config --global user.email yourname@example.com
```

This is important since your Git commits use this information.
The `--global` option ensures that you do not need to enter this information again on your machine.

It is convenient to set also the default text editor to use with Git (see below for 
more information on editors).
You can replace nano with vim, emacs or any other editor of your choice:
```shell
$ git config --global core.editor nano
```

We use a `git graph` alias very often (more info later).  Configure it
like this:
```shell
$ git config --global alias.graph "log --all --graph --decorate --oneline"
```


To see where this information is stored, use:
```shell
$ git config --list --show-origin
```

## Configuration problems

If you experience any configuration problems, please follow the 
[Software Carpentry troubleshooting guide](https://github.com/carpentries/workshop-template/wiki/Configuration-Problems-and-Solutions). 
If that still doesn't solve your problem, please write to support@coderefinery.org


## Text editor

Choosing the right text editor is a matter of taste and preferences. 
Since we often spend significant portions of our days editing text and source code, it can be 
valuable to invest time into learning your favourite editor really well. 
A few common options along with some pros/cons are given in 
[these instructions](https://coderefinery.github.io/installation/editors/).


