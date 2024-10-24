# tsbrowse-paper
This repository contains the manuscript, code and datasets accompanying the tsbrowse preprint (insert link).
It is organised as follows.

manuscript/
  figures/ #copies of high-resolution figures used in the manuscript
  manuscript_versions/ #copy of the Overleaf project containing manuscript, bibliography, latex template, styles etc
code/ #code used to create datasets and run inferences that the paper figures are based on.
datasets #for convenience, a copy of the input and output datasets discussed in the paper. 
  simulated_ARGs/
    sweep-simulated.trees #the simulated ARGs in tskit format discussed in Fig 2
    1000G-like-OOA-simulated.trees #the stdpopsim ARGs discussed in Supplementary Figure 2 (Panel A)
  inference_input/ #simulated ARGs converted to the input formats required by various inference software; can be reproduced with code
  inference_output/ #for convenience, output from inference software; code to produce is provided in code/
    sweep-tsinfer.trees #Supplementary Figure 1
    sweep-relate.trees #Supplementary Figure 1
    sweep-argneedle.trees #Supplementary Figure 1
    sweep-singer.trees #Supplementary Figure 1; SINGER makes a number of posterior sampled trees of which one is uploaded here
    1000G-chr20q-tsinfer.trees #Supplementary Figure 2 (Panel B), Supplementary FIgure 3

To install tsbrowse: 
  pip install tsbrowse #installs PyPi package
  python -m pip install git+https://github.com/tskit-dev/tsbrowse #installs development version
  
To run tsbrowse on the trees:
  python -m tsbrowse preprocess <path-to-input-trees> #preprocess input .trees or .tszip file; creates a .tsbrowse file in the input directory with the same prefix.
  python -m tsbrowse serve <path-to-input-tsbrowse> #serve the .tsbrowse file on a browser

For more information on tsbrowse see: https://github.com/tskit-dev/tsbrowse
Full documentation at: https://github.com/tskit-dev/tsbrowse/docs
