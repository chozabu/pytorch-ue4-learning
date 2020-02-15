# PytorchRL

This is a project trying out RL with pytorch and ue4

## setup

uses this branch of UE4Python: git@github.com:InterdimensionalGamesInc/UnrealEnginePython.git for 4.24 compat 
clone it into the projects Plugins folder (this should really be a sub-repo)

in windows, using global python env, packages:  
tensorflow-tensorboard==0.4.0rc3  
pytorch, using command from pytorch website  
more?

## usage

Working with this currently requires editing the python scripts to configure if there should be an attempt to load a model and continue training 
You will probably need to disable file loading.
Files are currently saved to a folder like "/Epic Games/UE_4.24/Engine/Binaries/Win64/NNModels"

## info

training is done "on the fly" in a background thread from physical instances of an agent, all sharing the same neural network

Network is TD3 based on this implementation: https://github.com/nikhilbarhate99/TD3-PyTorch-BipedalWalker-v2

relevant info: 
https://spinningup.openai.com/en/latest/  
Reinforcement Learning: An Introduction. Second edition, in progress. Richard S. Sutton and Andrew G. Barto  
unity-ml-agents




