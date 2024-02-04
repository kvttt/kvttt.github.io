---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

Contributions
-------------

1. ### *Contributed to [Project MONAI/MONAI](https://github.com/Project-MONAI/MONAI)*
    *  Opened and merged pull request [#7178](https://github.com/Project-MONAI/MONAI/pull/7178)
       in response to a feature request proposed in issue [#5484](https://github.com/Project-MONAI/MONAI/issues/5484),
       which adds a new `VoxelMorph` class to the existing MONAI Core and can serve as a general framework 
       based on which one can easily construct a deep learning network for 2D/3D image registration.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/Project-MONAI/MONAI/blob/dev/monai/networks/nets/voxelmorph.py)
    *  Opened and merged pull request [#7272](https://github.com/Project-MONAI/MONAI/pull/7272), 
       which adds a new registration regularizer `DiffusionLoss` in addition to the existing `BendingEnergyLoss`.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/Project-MONAI/MONAI/blob/dev/monai/losses/deform.py)
2. ### *Contributed to [Project MONAI/tutorials](https://github.com/Project-MONAI/tutorials)*
    *  Opened and merged pull request [#1566](https://github.com/Project-MONAI/tutorials/pull/1566), 
       which adds a tutorial on leveraging the newly implemented `VoxelMorph` class 
       to perform 3D image registration task on [Learn2Reg 2021](https://learn2reg.grand-challenge.org/Learn2Reg2021/) 
       Task 3 (OASIS dataset).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/Project-MONAI/tutorials/blob/main/3d_registration/learn2reg_oasis_unpaired_brain_mr.ipynb)
    *  Opened and merged pull request [#1589](https://github.com/Project-MONAI/tutorials/pull/1589), 
       which adds a notebook demonstrating the scaling laws 
       regarding the newly added `BendingEnergyLoss` and `DiffusionLoss`.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/Project-MONAI/tutorials/blob/main/modules/bending_energy_diffusion_loss_notes.ipynb)
 
Tools
-----

1. ### *PerfusionDSA*
    *  Created an interactive command line tool that takes as input a series of 2D$+t$ images 
       produced by cerebral X-ray Digital Subtraction Angiogram (DSA) and produces parametric images 
       including cerebral blood flow (CBF), cerebral blood volume (CBV), mean transit time (MTT), 
       and time to maximum flow-scaled residue function (Tmax).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/PerfusionDSA)
2. ### *N4BiasFieldCorrection*
    *  Created an easy-to-use command line tool that performs N4 bias field correction on a 3D volume 
       based on a [SimpleITK tutorial](https://simpleitk.readthedocs.io/en/master/link_N4BiasFieldCorrection_docs.html).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/N4BiasFieldCorrection)
3. ### *XRayPanorama*
    *  Created an interactive command line tool with simple GUI that, 
       given the hip, knee, and ankle images of the same subject, 
       stitches the three images together based on a [SimpleITK tutorial](https://github.com/SimpleITK/TUTORIAL/blob/main/07_registration_application.ipynb). 
       Additional functionalities were added to enhance the appearance of the resulting panorama.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/XRayPanorama)
4. ### *SpectralProfile*
    *  Created a little script that can be easily used on any PyTorch project to visualize the spectral profile 
       of a generated (or any) image (either 2D or 3D) based on Fast Fourier Transform (FFT).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/SpectralProfile)

Documentation
-------------

1. ### *OpenNFT-Note*
    *  Created a personal notebook of my experience with [Open-NFT](https://doi.org/10.1016/j.neuroimage.2017.06.039), 
       a Python/MATLAB-based tool for real-time fMRI neurofeedback training. 
       The notebook includes details from how to setup the environment to how to run a trial run 
       and is available both in Chinese and English.
    *  Read the Docs: [<img src="/images/logo-dark.png" width="25"/>](https://opennft-notes.readthedocs.io/en/latest/)