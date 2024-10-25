# tsbrowse-paper
This repository contains the manuscript, code and datasets accompanying the tsbrowse preprint (insert link). 
It is organised as follows.  
- code  *Code used to create datasets and run inferences for the paper figures*
        - datasets  *Input and output datasets discussed in the paper*
            - inference_input
                - test.haps
                - test.sample
                - test.vcf
            - inference_output  * Output from inference software; code to produce this is in the code/ directory *
                - sweep-tsinfer.trees   * Supplementary Figure 1 *
                - sweep-relate.trees    * Supplementary Figure 1 *
                - sweep-singer.trees    * Supplementary Figure 1; SINGER produces multiple posterior sampled trees; one is uploaded here *
                - 1000G-chr20q-tsinfer.trees    * Supplementary Figure 2 (Panel B), Supplementary Figure 3 *
            - simulated_ARGs    * Simulated ARGs converted to input formats for various inference software; reproducible with code *
                - sweep-simulated.trees * Simulated ARGs in tskit format discussed in Fig 2 *
                - 1000G-like-OOA-simulated.trees    * stdpopsim ARGs discussed in Supplementary Figure 2 (Panel A) *
        - manuscript
            - figures   * Copies of high-resolution figures used in the manuscript *
            - manuscript_versions   * Overleaf project containing the manuscript, bibliography, LaTeX template, styles, etc. *

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
