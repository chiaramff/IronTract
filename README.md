# IronTract

The repository contains the scripts used to run the standardized post-processing steps in the Round 2 of the IronTract Tractography Challenge.
https://irontract.mgh.harvard.edu

post_processing_script_Team1.py replicates the post-processing strategy of Team 1 in round 1. 
It implements a Gaussian filtering (sigma = 0.5) followed by an iterative thresholding of 200 steps on the log of the streamline count, for a total of 200 output tractogram volumes.

post_processing_script_Team2.py replicates the post-processing strategy of Team 2 in round 1. 
It retains only the streamlines passing through at least one of these ROIs: cingulum bundle,  genu of the corpus callosum,  external capsule,  anterior limb of the internal capsule, and the uncinate fasciculus. The ROIs were extracted from the PennCHOP Macaque atlas (Feng et al., Brain Struct Func, 2017)  are provided aligned to the space of the training and validation datasets. 
