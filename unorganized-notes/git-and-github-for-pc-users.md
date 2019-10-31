# Using Git and GitHub at GlobalGiving on a PC

Getting started with GitHub on a PC is a little different than with a Mac. Follow these instructions and you'll be just fine.

## Join GitHub

- If you don't already have an account [create one](https://github.com/join?source=header-home).

## Join the GlobalGiving organization

- Put in an Upkeep issue with Tech to be added to the GlobalGiving organization.
- @mention your manager in the issue to get them to comment with their consent to the request.
- Depending on your job description you may need to justify your reason for wanting access to the GlobalGiving organization

## Install Git

- First you need to know if your operating system is 32 bit or 64 bit. It's probably 64 bit but you should check.
  - Windows button --> settings gear --> About --> System
- [Download the right software here](https://git-scm.com/download/win)
- Change some settings as you step through the installer
  - "Select Components"
    - Make sure to check the box for Git Bash--it may already be checked
  - "Adjusting your path environment"
    - Use Git from Git Bash only
  - ""
    - Check out as-is, commit Unix style

## Set up your SSH key

- [GitHub's resource for this](https://help.github.com/articles/connecting-to-github-with-ssh/)
- Follow these instructions as closely as possible
  - As of 7/13/2018 there were no issues following these instructions

## Create the GlobalGiving idiomatic directory structure

At GlobalGiving we typically keep all of our work projects in subdirectories under `~/git/`
- Make that directory if you need to
```shell
mkdir ~/git
```

## Test & Practice

### Pull

- Create a test repo
- Clone it

### Fork

- Fork a remote repo
- Setup your fork as another remote

### Push

- Make some local changes
- Add, commit
- Push changes to your remote

### Pull Request

- Make a pull request from your remote to the origin
