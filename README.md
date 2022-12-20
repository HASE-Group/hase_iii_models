# Models

To checkout the model collection please use the following commands:

    git clone git@github.com:HASE-Group/hase_iii_models.git --recurse-submodules
    
        or
    
    git clone git@github.com:HASE-Group/hase_iii_models.git --recurse-submodules


# Notes on importing exising models

## To add a new model

Create a new repository for the model in https://github.com/orgs/HASE-Group/repositories

In the folder containing local copy of the model you want to push to github:

    git init
    git add *
    git commit -m "Added source for my super model!"
    git branch -M V1.0 
    git remote add origin git@github.com:HASE-Group/supermodel.git
    git push -u origin V1.0

This will push the new model onto github into the V1.0 branch.

## To add a new branch to an existing model continuing from the above

Create the new branch:

    git branch -M V1.1
    
Copy new files (ontop of old ones):

    cp -r ../../supermodel/V1.1/* ./ 
    
Remove any files you don't want any more after the above copy

Add and new files with git add command

    git add *
    
Use 'git status' to check you have added and removed the right files before committing (then use git add and git rm to add remove any desired files).

    git commit -m "Added source for V1.1 of my super model!"
    git push -u origin V1.1

## To add a new branch to an existing model using a new folder on your local machine

Start by cloning the prevous version to the new folder:

    gitclone -b V1.0 git@github.com:HASE-Group/supermodel.git supermodel
    
This clones all branches locally, and checksout the V1.0 branch into the V1.1 folder.

Then create a new branch (and switch to it):

    git branch -M V1.1
    
Copy new files (ontop of old ones)

    cp -r ../../supermodel/V1.1/* ./ 
    
Add and new files with git add command

    git add *

Use 'git status' to check you have added and removed the right files before committing (then use git add and git rm to add remove any desired files).

    git commit -m "Added source for V1.1 of my super model!"
    git push -u origin V1.1


# Notes on added a model to the models repo

First clone the models reposotry onto your local system:

    git clone git@github.com:HASE-Group/hase_iii_models.git --recurse-submodules

Then add a submodule for each model you wish to add

    git submodule add -b V3.5 git@github.com:HASE-Group/supermodel.git hase_iii_models/supermodel/V3.5
    
Commit the changes locally

    git commit -m "Added supermodel V3.5"
    
 Push the change back to github
 
    git push



