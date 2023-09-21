# NSSP
Welcome to NSSP! This repository will serve to give you all the code you will need for the class! If you made it this far, either through GitHub classroom or through direct link of this repository, well done, you're almost there!
This repo is meant to be useful to you, should you wish to save the work on your notebook!

# How to install
To get the code working properly, you must clone the repository and initialize the submodules as well! To do so:
```
git clone --recurse-submodules git@github.com:NX-421/access-class-s-repository-yourGitName.git
```
Take care to do this from within the virtual machine to access the notebooks.

# How to get week-to-week content
You need to call the following command:
```
git submodule update --remote
```

# Launching a notebook
Because we use a special environment to display the fMRI images, you will need to launch the notebook with a special syntax as well. Within a terminal, you must navigate to the directory of your notebook. For example if you want to run the notebook of /some/path/Week5/lab_5.ipynb, the command would be:

```
fsleyes --notebookFile /some/path/Week5/lab_5.ipynb
```

You can find a cheatsheet here for all above commands and some useful git commands as well:
https://docs.google.com/presentation/d/1CchGL0nTBvvp9yCJcaZnByDCfcygVsCg1fs_1OriLeM/edit?usp=sharing
