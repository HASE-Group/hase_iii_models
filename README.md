# models
To checkout the model collection please use the following commands:

    git clone https://github.com/HASE-Group/models.git --recurse-submodules
    
        or
    
    git clone git@github.com:hase-group/models.git --recurse-submodules



# Notes on importing exising models

-- To add a new model:

Create a new repository for the model in https://github.com/orgs/HASE-Group/repositories

On the local copy of the model you want to push to github:

  git init
  git add *
  git commit -m "Added source for my super model!"
  git branch -M V1.0 
  git remote add origin git@github.com:HASE-Group/supermodel.git
  git push -u origin V1.0

This will push the new model onto github into the V1.0 branch.

-- To add a new branch to an existing model continuing from the above:

Create the new branch
  git branch -M V1.1
  cp -r ../../supermodel/V1.1 ./ 
Remove any files you don't want any more after the above copy
Add and new files with git add command
Use 'git status' to check you have added and removed the right files before committing.
  git commit -m "Added source for V1.1 of my super model!"
  git push -u origin V1.1


-- To add a new branch to an existing model using a new folder on your local machine:

Start by cloning the prevous version to the new folder
  gitclone -b V1.0 git@github.com:HASE-Group/mips1.git V1.1
This clones all branches locally, and checksout the V1.0 branch into the V1.1 folder.
Then create a new branch (and switch to it):
  git branch -M V1.1
Copy files
  cp -r ../../supermodel/V1.1 ./ 
Add and new files with git add command
Use 'git status' to check you have added and removed the right files before committing.
  git commit -m "Added source for V1.1 of my super model!"
  git push -u origin V1.1

