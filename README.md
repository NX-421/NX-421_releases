# NSSP
Welcome to NSSP! This repository will serve to give you all the code you will need for the class! If you made it this far, either through GitHub classroom or through direct link of this repository, well done, you're almost there!
This repo is meant to be useful to you, should you wish to save the work on your notebook!

Note that we **only support the virtual machine**. Remember to always connect to EPFL VPN if working from home! 
You can download the VM client [here](http://vdi.epfl.ch). Once you install it, click New Server, enter vdi.epfl.ch and click connect. This will add EPFL's VDI portal to your VMWare.
You should then be able to click on it, and login with your GASPAR to get access to all of the VMs EPFL makes available for you.
Our VM is the one called NX-421. Click on it, and it should boop a VM for you where you can start working!

## Setting up your GitHub account in the virtual machine
To authenticate to your repository, you will need your GitHub account to be setup within the VM. Nothing hard! Simply run _(with the quotation marks)_ from a terminal _(which you can open by pressing ctrl + alt + t )_:
```
git config --global user.name "yourGitAccountName"
git config --global user.email "yourGitEmail@example.com"
```

If you're using SSH to identify to GitHub (which we advise), you will need to create a new SSH authentication key from within the virtual machine or copy both your public and private ssh key on the VM (we advise strongly against this copy: create a new set of keys to be secure).

Note that these steps need only be done once, as the VM will save those settings as your user settings.


## How to install
To get the code working properly, you must clone the repository and initialize the submodules as well! To do so:

```
git clone --recurse-submodules git@github.com:NX-421/access-class-s-repository-yourGitName.git
```
Take care to do this from within the virtual machine to access the notebooks.

## How to get week-to-week content
You need to call the following command:
```
git submodule update --remote
```

## Launching a notebook
Because we use a special environment to display the fMRI images, you will need to launch the notebook with a special syntax as well. Within a terminal, you must navigate to the directory of your notebook. For example if you want to run the notebook of /some/path/Week5/lab_5.ipynb, the command would be:

```
fsleyes --notebookFile /some/path/Week5/lab_5.ipynb
```

You can find a cheatsheet here for all above commands and some useful git commands as well:
https://docs.google.com/presentation/d/1CchGL0nTBvvp9yCJcaZnByDCfcygVsCg1fs_1OriLeM/edit?usp=sharing
