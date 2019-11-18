# Using Git and GitHub on a PC

Getting started with GitHub on a PC is a little different than with a Mac. Follow these instructions and you'll be just fine.

## Join GitHub

- If you don't already have an account [create one](https://github.com/join?source=header-home).

## Install Git

- First you need to know if your operating system is 32 bit or 64 bit. It's probably 64 bit but you should check.
  - Windows button --> settings gear --> About --> System
- [Download the right software here](https://git-scm.com/download/win)
- Change some settings as you step through the installer
  - "Select Components"
    - Make sure to check the box for Git Bash--it may already be checked
  - "Adjusting your path environment"
    - Use Git from Git Bash only
  <!-- TODO: need to figure out what this instruction was -->
  - ""
    - Check out as-is, commit Unix style

## Set up your SSH key

- [GitHub's resource for this](https://help.github.com/articles/connecting-to-github-with-ssh/)
  - [Here's another tutorial that is specific to Windows 10](https://tutorials.ubuntu.com/tutorial/tutorial-ssh-keygen-on-windows#0)
- Follow these instructions as closely as possible

## Test

- Try running `git clone git@github.com/bcope/gobble`
