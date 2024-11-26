# tsbrowse-paper
This repository contains the manuscript, code and datasets accompanying the tsbrowse preprint (insert link). 
It is organised as follows.  
- code *Code used to create datasets and run inferences for the paper figures*
- manuscript
    - figures *Copies of high-resolution figures used in the manuscript*
    - manuscript_versions *Overleaf project containing the manuscript, bibliography, LaTeX template, styles, etc.*

#### To install tsbrowse:  
    pip install tsbrowse #installs PyPi package  
    python -m pip install git+https://github.com/tskit-dev/tsbrowse #installs development version  
  
#### To run tsbrowse on the trees:  
    python -m tsbrowse preprocess <path-to-input-trees> #preprocess input .trees or .tszip file; creates a .tsbrowse file in the input directory with the same prefix.  
    python -m tsbrowse serve <path-to-input-tsbrowse> #serve the .tsbrowse file on a browser  
  
#### For more information on tsbrowse: 
    https://github.com/tskit-dev/tsbrowse  
#### Full documentation: 
    https://github.com/tskit-dev/tsbrowse/docs  
