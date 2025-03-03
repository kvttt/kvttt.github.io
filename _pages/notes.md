---
layout: archive
title: "Notes"
permalink: /notes/
author_profile: true
---


On Microstructure Imaging
-------------------------

1. ### *Causality of the diffusion propagator*
    *  Developed a 4-page note that provides both an intuitive and mathematical explanation of the causality of the diffusion propagator.
    *  Fun fact: the content of this note was inspired by an integral problem Dmitry asked me to solve during my interview with him at NYU.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/causality.pdf)


On MR Physics
-------------

1. ### *Bloch Equations*
    *  Developed a 3-page note showing how one can derive the Bloch Equations from basic eletromagnetism and classical mechanics, along with some mild assumptions about the nature of \\(T_1\\) and \\(T_2\\) relaxation.
    *  The note also demonstrates how one can find an exact solution to the Bloch Equations in the case of free induction decay (FID).
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/Bloch_Equations.pdf)


On Deep Learning
----------------

1. ### *A Collection of Frequently Asked Questions about Denoising Diffusion Probabilistic Models*
    *  Developed an 8-page note that explains some of the most important concepts regarding denoising diffusion probabilistic models (DDPMs).
    *  The note mainly seeks to answer two questions:
        *  Does the forward process tend to \\(\mathcal{N}(\mathbf{0}, \mathbf{I})\\)?
        *  How do you get from NLL to \\(L_\mathrm{simple}\\)?
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/DDPM_FAQ.pdf)

2. ### *Faster Convolution*
    *  Developed an 8-page note introducing an alternative implementation of the convolution operation 
       that is faster than the traditional convolution operation in some cases. The note also provides 
       in-depth comparison between the traditional convolution operation and the proposed faster convolution operation.
    *  The note includes:
        *  A pseudocode outlining the alternative implementation.
        *  A Python implementation.
        *  Detailed experimental settings and detailed results including total CUDA times and CUDA time for each underlying operation.
    *  The note offers insight into when and how to accelerate convolution operations during training/inference.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/Faster_Convolution.pdf)


On Spherical Harmonics
----------------------

1. ### *Spherical Harmonics Fitting*
    *  Developed a 7-page note which serves as an accompanying note for the MATLAB toolbox 
       [Spherical Harmonics Fitting](https://www.mathworks.com/matlabcentral/fileexchange/168591-spherical-harmonics-fitting).
    *  The note covers both the technical and practical aspects of spherical harmonics fitting.
        *  The technical aspect includes three different formulations of the least squares problem associated with spherical harmonics fitting and the derivation of a regularizer.
        *  The practical aspect includes line-by-line explanation of the usage of the toolbox using a simple example of reconstructing a tensor-valued orientation distribution function (ODF).
    * Note: [<img src="/images/pdf.png" width="25"/>](/files/Spherical_Harmonics_Fitting.pdf) 


On Statistical Estimation
-------------------------

1. ### *Score Matching*
    *  Developed a 6-page note that provides an in-depth explanation of [score matching](https://www.jmlr.org/papers/volume6/hyvarinen05a/hyvarinen05a.pdf).
    *  The note provides more detailed explanations of the theorems presented in the paper with elementary but more rigorous proofs, which include:
        * Theorem 1: Simplification of the objective function. 
        * Theorem 2: Well-definedness of the estimator obtained by minimization of the exact objective function.
        * Corollary 3: Consistency of the estimator obtained by minimization of the approximated objective function based on sampling.
    *  The note also includes explanation of the motivation behind score matching and clarification of some of the mild yet essential regularity assumptions omitted by the author.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/Score_Matching.pdf)


On Ill-posed Inverse Problems
-----------------------------

1. ### *Tikhonov Regularized Linear Problem*
    *  Developed a 6-page note on providing four different interpretations of Tikhonov regularization, which includes
        1. Two interpretations from the standpoint of linear algebra,
        2. One front a geometric perspective, and
        3. One statistical interpretation.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/Tikhonov_Regularized_Linear_Problems.pdf) 

2. ### *Plug-and-Play ADMM using MATLAB and PyTorch*
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


On Medical Image Registration
-----------------------------

1. ### *Converting ANTs affine matrix to a \\(4 \times 4\\) homogeneous matrix*
    *  Developed a 4-page note that demonstrates two methods of converting an affine matrix
       obtained from ANTs to a \\(4 \times 4\\) homogeneous matrix,
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


On Mathematical Analysis
----------------

1. ### *Review Notes for MATH 754: Introductory Functional Analysis*
    * Developed a 12-page note that summarizes the materials covered in MATH 754: Introductory Functional Analysis so far, 
      a graduate-level functional analysis course I am currently taking.
    * Topics covered in this note include:
      * Finite dimensional normed spaces
      * Hilbert spaces
      * Banach spaces
      * Fréchet spaces
      * Topological vector spaces
      * Duality
    * Main theorems include:
      * Riesz Representation theorem
      * Riesz-Fisher theorem
      * Hahn-Banach theorem
      * Banach-Alaoglu theorem
    * This note is a work in progress. Stay tuned!

2. ### *All Hilbert spaces are \\(\ell^2-\\)spaces*
    *  Developed a 4-page note that made explicit the sense in which all Hilbert spaces are \\(\ell^2-\\)spaces.
    *  I will continue filling in the proofs and examples in the future. Stay tuned!
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/hilbert_l2.pdf)

3. ### *Review Notes for MATH 653: Introductory Analysis*
    *  Developed a 34-page note that summarizes the materials covered in MATH 653: Introductory Analysis, 
       a graduate-level analysis course I have taken during my senior year at UNC-Chapel Hill.
    *  Topics covered in this note include:
       *  Metric spaces
       *  Basics of measure theory
       *  Lebesgue integration theory
       *  Compactness in function spaces
       *  Density and approximation in function spaces
       *  Existence and uniqueness for systems of ODEs
       *  Complex analysis
    *  The aim of this note is to organize the materials in a way that is easy to understand and to provide
       a quick reference when studying for midterms and finals.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/653-notes.pdf)

4. ### *Review Notes for MATH 522: Advanced Calculus II*
    *  Developed a 40-page note that summarizes the materials covered in MATH 522: Advanced Calculus II.
    *  Topics covered in this note include:
       *  Metric spaces
       *  Jordan content and Riemann integration
       *  Differential forms
       *  Surfaces
       *  ODE theory
       *  Lebesgue measure and integration
    *  The aim of this note is to organize the materials in a way that is easy to understand and to provide
       a quick reference when studying for midterms and finals.
    *  Note: [<img src="/images/pdf.png" width="25"/>](/files/522-notes.pdf)

[//]: # (<br/><br/><br/><br/><br/><br/><br/><br/><br/>)
