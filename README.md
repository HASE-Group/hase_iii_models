# Models

Simulation models of a variety of computer architectures and architectural components have been created using HASE, a Hierarchical Computer Architecture design and Simulation Environment. These models are intended for use as teaching and learning resources: in lectures, for student self-learning or for virtual laboratory experiments.

Using the models requires use of HASE itself. The latest version of HASE is available for Linux, MAC OSX and Windows and can be downloaded from https://github.com/HASE-Group/hase_iii_releases

Each model has its own supporting documentation describing the system being modelled as well as the model itself. These model files provide the input to HASE which has options to load a project, to compile a simulation executable and to run the simulation. Running a simulation produces a trace file which can be used to animate the on-screen display of the model so as to show data movements, parameter value updates, state changes, etc.

This repository contains a collection of "official" supported HASE3 models. Each model and its documentation can be found in a folder of the model’s name. The model subfolder contains the documentation about each model and its versions. The sub folders in each model folder contain git submodules (references) to the model sources (each model is stored in its own repo with its own branches).

To checkout the model collection please use the following commands:

    git clone git@github.com:HASE-Group/hase_iii_models.git --recurse-submodules
    
        or
    
    git clone git@github.com:HASE-Group/hase_iii_models.git --recurse-submodules

## Released Models

The following computer architecture models are currently available inside this collection:

- Manchester Small Scale Experimental Machine
- Cray-1
- CDC 6600
- Atlas (the Manchester University / Ferranti Atlas computer, inaugurated December 1962)
- MU5 (the fifth major computer system built at Manchester University)


