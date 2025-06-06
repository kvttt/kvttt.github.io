---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---


Contributions
-------------

1. ### *Contributed to [mfuderer/colorResources](https://github.com/mfuderer/colorResources)*
    *  Opened and merged pull request [#9](https://github.com/mfuderer/colorResources/pull/9), 
       which adds a Python reimplementation of the recommended color-map for MR relaxometry maps 
       by the Quantitative MR Study Group of the International Society for Magnetic Resonance in Medicine (ISMRM).
    *  For additional details, check out [Color-map recommendation for MR relaxometry maps](https://onlinelibrary.wiley.com/doi/10.1002/mrm.30290).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/mfuderer/colorResources/blob/main/exampleUse.py)

2. ### *Contributed to [DIPY/DIPY](https://github.com/dipy/dipy)*
    *  Opened and merged pull request [#3237](https://github.com/dipy/dipy/pull/3237), 
       which deprecates the old `interp_rbf` function, which only supports interpolation of scalar-valued spherical functions,
       and replaces it with a new `rbf_interpolation` function that supports interpolation of tensor-valued spherical functions.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/dipy/dipy/blob/master/dipy/core/interpolation.pyx)

3. ### *Contributed to [Project MONAI/tutorials](https://github.com/Project-MONAI/tutorials)*
    *  Opened and merged pull request [#1566](https://github.com/Project-MONAI/tutorials/pull/1566), 
       which adds a tutorial on leveraging the newly implemented `VoxelMorph` class 
       to perform 3D image registration task on [Learn2Reg 2021](https://learn2reg.grand-challenge.org/Learn2Reg2021/) 
       Task 3 (OASIS dataset).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/Project-MONAI/tutorials/blob/main/3d_registration/learn2reg_oasis_unpaired_brain_mr.ipynb)
    *  Opened and merged pull request [#1589](https://github.com/Project-MONAI/tutorials/pull/1589), 
       which adds a notebook demonstrating the scaling laws 
       regarding the newly added `BendingEnergyLoss` and `DiffusionLoss`.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/Project-MONAI/tutorials/blob/main/modules/bending_energy_diffusion_loss_notes.ipynb)

4. ### *Contributed to [Project MONAI/MONAI](https://github.com/Project-MONAI/MONAI)*
    *  Opened and merged pull request [#7178](https://github.com/Project-MONAI/MONAI/pull/7178)
       in response to a feature request proposed in issue [#5484](https://github.com/Project-MONAI/MONAI/issues/5484),
       which adds a new `VoxelMorph` class to the existing MONAI Core and can serve as a general framework 
       based on which one can easily construct a deep learning network for 2D/3D image registration.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/Project-MONAI/MONAI/blob/dev/monai/networks/nets/voxelmorph.py)
    *  Opened and merged pull request [#7272](https://github.com/Project-MONAI/MONAI/pull/7272), 
       which adds a new registration regularizer `DiffusionLoss` in addition to the existing `BendingEnergyLoss`.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/Project-MONAI/MONAI/blob/dev/monai/losses/deform.py)

Tools
-----

1. ### *Cortical Surface Quality Control*
    *  Created a tool for quality control of cortical surfaces (both pial and white surfaces with cortical thickness and curvature overlaid).
    *  The tool creates PDFs containing visualized cortical surfaces, and corresponding CSV files for experts to performance quality assessment.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/Cortical_Surface_QC)
    ![QC](/images/QC.png)

2. ### *Pituitary Segmentation*
    *  Created an atlas-based command-line segmentation tool for automatic pituitary segmentation in 3D MR images. 
       The tool is based on the [MNI152 2009a Nonlinear Asymmetric atlas](https://www.bic.mni.mcgill.ca/ServicesAtlases/ICBM152NLin2009)
       and a corresponding pituitary mask annotated by a radiologist.
    *  Added functionality
        *  Now providing the option to use multiple atlases for more robust segmentation results. 
        *  The new command-line tool is written entirely in bash without dependency on Python and is based on the C++-based ANTs (instead of ANTsPy).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/Pituitary_Segmentation)

3. ### *Spherical Harmonics Fitting*
    *  Re-implemented selected tools from DIPY for fitting spherical harmonics in DIPY.
       In addition, a helpful tool for converting gradient directions `bvec` from the 
       Cartesian coordinate system to the corresponding spherical coordinate system was also implemented.
       The re-implementation offers the same functionality as the original DIPY tools 
       but allows the user to directly run the tools from MATLAB without dependency on DIPY.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/Spherical-Harmonics-Fitting)
    *  MATLAB File Exchange: [![View Spherical Harmonics Fitting on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/168591-spherical-harmonics-fitting)
    ![SH](/images/SH.jpg)

4. ### *Patch2Self_MATLAB*
    *  Re-implemented Patch2Self in MATLAB based on the [original paper](https://arxiv.org/abs/2011.01355) 
       and the [official DIPY implementation](https://github.com/dipy/dipy/blob/master/dipy/denoise/patch2self.py). 
       Patch2Self is a widely used self-supervised learning method for denoising diffusion MRI data. 
       However, the use case of my current project (and many others) requires running Patch2Self as part of a MATLAB pipeline.
       Re-implementation of Patch2Self in MATLAB allows for seamless integration of Patch2Self into such pipeline.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/Patch2Self_MATLAB)
    *  MATLAB File Exchange: [![View Patch2Self_MATLAB on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/168596-patch2self_matlab)

5. ### *ICON_OASIS*
    *  A reproduction of ICON and GradICON on the OASIS dataset 
       based on the [ICON original paper](https://arxiv.org/abs/2105.04459) and [GradICON original paper](https://arxiv.org/abs/2206.05897). 
       This re-implementation uses `MONAI.networks.nets.VoxelMorph` and `MONAI.losses.DiffusionLoss`. 
       The purpose of this project is to try out [Marc's group's](https://biag.cs.unc.edu/author/marc-niethammer/) latest work 
       and provide an example of how to integrate the ICON and GradICON loss functions into an existing training pipeline.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/ICON_OASIS)

6. ### *UnstructuredInterpolation*
    *  Created a utility for unstructured interpolation of 2D/3D data 
       at any number of arbitrary locations based on `torch.nn.functional.grid_sample`. 
       Cases where this is useful include applying a displacement field 
       predicted at discrete voxel locations to a densely and continuously sampled surface 
       represented by a set of vertices.
    * GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/UnstructuredInterpolation)

7. ### *PerfusionDSA*
    *  Created an interactive command line tool that takes as input a series of 2D$+t$ images 
       produced by cerebral X-ray Digital Subtraction Angiogram (DSA) and produces parametric images 
       including cerebral blood flow (CBF), cerebral blood volume (CBV), mean transit time (MTT), 
       and time to maximum flow-scaled residue function (Tmax).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/PerfusionDSA)

8. ### *N4BiasFieldCorrection*
    *  Created an easy-to-use command line tool that performs N4 bias field correction on a 3D volume 
       based on a [SimpleITK tutorial](https://simpleitk.readthedocs.io/en/master/link_N4BiasFieldCorrection_docs.html).
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/N4BiasFieldCorrection)
    *  Here is a T1 MPRAGE image of my brain before and after N4 bias field correction:
    ![N4](/images/N4.png)

9. ### *XRayPanorama*
    *  Created an interactive command line tool with simple GUI that, 
       given the hip, knee, and ankle images of the same subject, 
       stitches the three images together based on a [SimpleITK tutorial](https://github.com/SimpleITK/TUTORIAL/blob/main/07_registration_application.ipynb). 
       Additional functionalities were added to enhance the appearance of the resulting panorama.
    *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/XRayPanorama)

10. ### *SpectralProfile*
     *  Created a little script that can be easily used on any PyTorch project to visualize the spectral profile 
        of a generated (or any) image (either 2D or 3D) based on Fast Fourier Transform (FFT).
     *  GitHub: [<img src="/images/github-mark.png" width="25"/>](https://github.com/kvttt/SpectralProfile)


Documentation
-------------

1. ### *OpenNFT-Note*
    *  Created a personal notebook of my experience with [Open-NFT](https://doi.org/10.1016/j.neuroimage.2017.06.039), 
       a Python/MATLAB-based tool for real-time fMRI neurofeedback training. 
       The notebook includes details from how to set up the environment to how to run a trial run 
       and is available both in Chinese and English.
    *  Read the Docs: [<img src="/images/logo-dark.png" width="25"/>](https://opennft-notes.readthedocs.io/en/latest/)
