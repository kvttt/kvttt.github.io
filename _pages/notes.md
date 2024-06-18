---
layout: archive
title: "Notes"
permalink: /notes/
author_profile: true
---

On Ill-posed Inverse Problems
-----------------------------

1. ### *Plug-and-Play ADMM using MATLAB and PyTorch*
    *  Developed a 6-page tutorial on how to implement the Plug-and-Play ADMM algorithm using MATLAB and PyTorch.
    *  MATLAB is used to for solving the regularized least-squares problem associated with the first step.
    *  PyTorch is used to export a pre-trained denoiser model, which is plugged into the ADMM algorithm.
    *  Besides providing a step-by-step guide on how to implement the algorithm, 
       the aim of this tutorial is three-fold: 
        1. To explain one of the caveats of running python scripts in MATLAB.
        2. To compare the performance and convergence property of `lsqr` for the original problem 
           and `pcg` for the corresponding normal problem.
        3. To provide a template for handling variable passing between MATLAB and PyTorch via ProtoBuf.
      * In addition, the tutorial also provides a brief introduction and problem formulation of the Plug-and-Play ADMM algorithm
        from a mathematical perspective.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/PnP_ADMM.pdf) 

Medical Image Registration
--------------------------

1. ### *Converting ANTs affine matrix to a $4 \times 4$ homogeneous matrix*
    *  Developed a 4-page note that demonstrates two methods of converting an affine matrix
       obtained from ANTs to a $4 \times 4$ homogeneous matrix,
       which can be subsequently incorporated into a pipeline
       dealing with both image volumes and surfaces.
    *  The aim of this note is to provide a clear and concise explanation of the mathematical
       concepts behind this seemingly simple yet sometimes frustrating procedure,
       to facilitate the understanding of the relationship between LPS and RAS spaces,
       and to provide a practical example of how to perform the conversion.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/ANTs_mat.pdf)
2. ### *Deformable Image Registration*
    *  Developed a 2-page note that clarifies notations and concepts that are frequently abused and confused
       in the field of deformable image registration. 
    *  The note also provide definitions of important terms and their mathematical formulations.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/Registration.pdf)

Mathematics
-----------

1. ### *Review Notes for MATH 522: Advanced Calculus II*
    *  Developed a 40-page note that summarizes the materials covered in MATH 522: Advanced Calculus II.
    *  Topics covered in this note includes: 
       *  Metric spaces
       *  Jordan content and Riemann integration
       *  Differential forms
       *  Surfaces
       *  Functional analysis
       *  ODE theory
       *  Lebesgue measure and integration
    *  The aim of this note is to organize the materials in a way that is easy to understand and to provide
       a quick reference when studying for midterms and finals.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/522-notes.pdf)
