# Session 1 - Getting Installed and Running Hello World

## Pre-work - Getting Ready

### All Platforms

- **Have a computer you can install things on**
  - **Bring a power cord**
- Sign up for an account on [GitHub](https://github.com/join)
  - Use your personal email address
  - Consider making your username something you would be okay putting on your resume
- Download [VSCode](https://code.visualstudio.com/download)
  - Install <!-- TODO: add specifics that choices that should be made during install -->

### PC

- Download [git](https://git-scm.com/downloads)
  - Wait to install--you may already have this

## Intro

The goal for today is to muscle through the dirty work of installing requirements and produce a runnable program.

You will hear things you don’t understand yet. You will need to get comfortable with semi- or non-understandings. In this session we will quickly perform some tasks without a thorough explanation. This is in order to get to the fun part quickly and not get bogged down.

Write down any questions you have and we can get back to them later.

## Goals

- Install VSCode
- Install git
- Get python 3 installed
- Get Jupyter installed
- Run “Hello World” from a Jupyter notebook
- Write a “Hello World” python script and execute from the command line

## A Note on Python Versions

Python 2 and Python 3 are not equivalent. We'll be using Python 3. Your computer may have Python 2.7.x on it already--you still need to install Python 3. I'll be using Python 3.7.4 but the difference between subversions of Python 3 are irrelevant to what we'll be doing here.

## OS Specific Install Instructions

### Mac

#### The `pyenv` method

This is the best way (that I know of) to install python 3. This method is recommended by [this blogpost](https://opensource.com/article/19/5/python-3-default-mac#what-we-should-do).

Conceptually we are using a package manager (`brew`) to install what is essentially a package manager (`pyenv`) which we'll use to install a specific version of Python.

1. Install `brew`
    1. Open the terminal
    1. Run the following command: `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
    1. You may need to enable or install Xcode
1. Use `brew` to install `pyenv`
    1. Run the following command `brew install pyenv`
1. Use `pyenv` to install python 3
    1. Run `pyenv install 3.8`
1. Now that Python 3 is installed through pyenv, we want to set it as our global default version for pyenv environments
    1. Run `pyenv global 3.8`
    1. Verify that it worked
        1. Run `pyenv version`
1. Copy/download the files `bashrc` and `bash_profile` into your home directory
    1. Run the following:
        ```sh
        if [ -s "~/.bashrc" ]; then echo "You already have a .bashrc file in your home directory"; else curl https://gist.githubusercontent.com/bcope/3733714df0615813c2eca685de1106c4/raw/10d76dc7dff3708c465327e68bce5eac272e18bd/bashrc_template.sh >> ~/.bashrc; fi; if [ -s "~/.bash_profile" ]; then echo "You already have a .bash_profile file in your home directory"; else curl https://gist.githubusercontent.com/bcope/462d6ea91964f6be6aef3d8f840c369b/raw/43c6fd77ae47d48f22440ba9ac056f98bb38651b/bash_profile_template.sh >> ~/.bash_profile; fi
        ```
1. Close the terminal and open again
1. Verify that primary version of python is being run by pyenv
    1. Run `which python`
    1. You should see something like `/Users/<your-username>/.pyenv/shims/python`. The important part is the `.pyenv` in the middle
1. Verify the python version
    1. Run `python --version`. It should be 3.8
1. Verify the pip version
    1. Run `pip --version`
    1. You should see something like `pip 19.0.3 from /Users/<your-username>/.pyenv/versions/3.8/lib/python3.8/site-packages/pip (python 3.8)`
1. Check to see if git is installed
    1. Run `git --version`
    1. If not, try installing using brew: `brew install git`

### PC

1. Install git
    1. **Make sure to install Git Bash**
1. Open Git Bash
    1. Alternatively you could use Windows Command Prompt but for the purposes of this workshop we’re using Git Bash so that the commands we type will be the same across platforms
1. Check to if python is installed and on the PATH
    1. Run `python --version`
1. Install python 3 if necessary
    1. Download python 3
    1. Make sure to check the box that adds Python 3 to your path.

### Chromebook

Full disclosure, I have no idea if this workshop will be able to be done locally on a Chromebook. It might be the case that we'll have to use a remote, web-based dev environment.

1. Open the Crosh shell
    1. `ctrl + alt + t`
1. Possible next step...
    1. https://www.wsvincent.com/install-python3-chromebook/

## Cross Platform Instructions

1. Install VSCode if you haven't already
1. Create some folders
    1. In the terminal create a directory for us to store all our code
        1. Run `mkdir ~/git`
    1. Open that directory by running the change director command
        1. Run `cd ~/git`
    1. Now make a directory for us to store our hello world program that we’ll write later
        1. Run `mkdir hello-world`
1. Pip install jupyter notebooks
    1. Run `pip install jupyter`
1. Write hello world program in a Jupyter Notebook <!-- TODO: put instructions here -->
1. Write hello world program in VSCode <!-- TODO: put instructions here -->

## Bonus

1. Try updating the terminal to look the way you want
1. Install plugins for VSCode
    1. Atom Keymap - I recommend this so that we can be using the same keyboard shortcuts
    1. Live Share - this could come in handy later
    1. Python - syntax highlighting etc
    1. vscode-icons - makes files easier to differentiate by type

## Questions

## Concepts

- Command line
  - Navigation using `cd`
  - Creating directories with `mkdir`
- Pip
  - Used to install python specific libraries
