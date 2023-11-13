# PySnacks 5<br> ASTROALIGN: A python pipeline to explore space-based observations in the search for planets
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/iaa-so-training/pysnacks5_astroalign/HEAD)


This repository is for the workshop materials. For details on the event visit the [PySnacks 5: ASTROALIGN](https://indico.iaa.csic.es/event/8/) event webpage.
![image](https://github.com/iaa-so-training/pysnacks5_astroalign/assets/1053066/da43ad82-77aa-4c8a-9363-40b4a0d43214)

## PySnacks
Within the  Severo Ochoa Training Initiative of the IAA-CSIC we are offering short introductory practical courses about Python packages for astrophysical applications (PySnacks). We invite you to participate in the 1h course PySnacks 5: ASTROALIGN.

 
## Abstract
ASTROALIGN is a python module that can serve to align two astronomical images. It determines the solution  by finding similar 3-point asterisms (triangles) in both images and estimating the affine transformation between them. ASTROALIGN is particularly useful when there is no WCS information available or when the images to be aligned have been taken at different wavelengths and initial “by eye” alignment is very challenging. In this 1h workshop I will impart  a brief  introduction into the capabilities of ASTROALIGN and how to use it.
 
This course will be taught by Rainer Schödel. 

## Workshop materials
There are mainly three tutorials:

- [tutorials/Astroalign_Example.ipynb](tutorials/Astroalign_Example.ipynb)
- [tutorials/Example_GNS/AA_with_lists.ipynb](tutorials/Example_GNS/AA_with_lists.ipynb)
- [tutorials/Example_JPEG/AA_with_jpg.ipynb](tutorials/Example_JPEG/AA_with_jpg.ipynb)

The file structure is:
```
├── environment.yml
├── LICENSE
├── README.md
└── tutorials
    ├── Astroalign_Example.ipynb
    ├── Example_GNS
    │   ├── AA_with_lists.ipynb
    │   ├── HAWKI_H_lnx_jitter_3.fits.gz
    │   ├── HAWKI_H_stars_3.txt
    │   ├── VVV_J_Field5.fits.gz
    │   └── VVV_J_Field5_stars.txt
    └── Example_JPEG
        ├── AA_with_jpg.ipynb
        ├── detail.jpg
        ├── eso1547a.jpg
        └── orig.jpg
```

# Installation instructions
You can manage the instalation with `conda` following these steps:

1. Make sure you have conda/mamba installed. You can follow the instructions in [Installing miniconda](https://droplets-spsrc.readthedocs.io/conda/#installing-miniconda).

2. In a terminal, go to your working directory and clone this repository:

```
git clone https://github.com/iaa-so-training/pysnacks5_astroalign.git
cd pysnacks5_astroalign
```


3. Install the dependencies for the tutorials (replace `mamba` with `conda` if you don't have mamba installed):
```
mamba env create -f environment.yml
```

4. Execute the tutorials

You need to activate the conda environment and initialize a Jupyter Lab session:

```
conda activate astroalign
jupyter lab
```

Once everything is installed, you just need to run step 4 to run the tutorials.

You can also launch the tutorials without installation in the free myBinder service by clicking here: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/iaa-so-training/pysnacks5_astroalign/HEAD). Note that this is a free service with limited resources, useful to execute and modify the tutorials live, but computationally expensive steps may not be possible.

## Additional information
 - ASTROALIGN paper: https://arxiv.org/abs/1909.02946
 - ASTROALIGN documentation: https://astroalign.quatrope.org/en/latest/  
