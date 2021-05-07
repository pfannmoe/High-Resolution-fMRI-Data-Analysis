# High-Resolution-fMRI-Data-Analysis

These are Matlab Scripts for high resolution fMRI data analysis with FreeSurfer. We recommend the use of the Multi-Echo-MPRAGE sequence for T1w imaging of the brains anatomy 
(A.J.W. van der Kouwe, T. Benner, D.H. Salat, and B. Fisch (2008) Brain morphometry with multiecho MPRAGE. Neuroimage;40(2):559-569) optimized for the FreeSurfer anatomical 
reconstruction of white and gray matters surfaces. Although the approach also works with any other sequence for imaging of the anatomy. This tool offers an improved spatial 
specificty of your data analysis compared to standard FS-FAST based on a new approach in the fMRI data preprocessing that takes into account the position of each voxel in the fMRI time series. Details of the data analysis are outlined in: 

(J. Härtner, S. Strauss, J. Pfannmöller, and M. Lotze (2021) Tactile acuity of fingertips and hand representation size in human Area 3b and Area 1 of the primary somatosensory cortex. NeuroImage; 232: 117912) and (J. Pfannmoeller, S. Strauss, I. Langner, T. Usichenko, and M. Lotze (2019) Investigations on maladaptive plasticity in the sensorimotor cortex of unilateral upper limb CRPS I patients. Restorative Neurology and Neuroscience;37: 143–153).

These Matlab scripts have been written for use on a linux machine with Freesurfer 6 installed. The first step of the data analysis is the segmentation of brain 
anatomy with the Freesurfer recon-all command. After that you need to generate a directory structure as outlined in the scripts. The scripts can then be used to execute the 
data analysis. It is advisable to check the quality of the registration using the script having B_ as prefix. You will always have an improved spatial specificity in your 
fMRI data analysis compared to FS-FAST. The voxel size of your fMRI data determines how much the spatial specificity of your data analysis will improve. 
