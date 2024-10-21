# Multi-Layer-Gaussian-Splatting-for-Immersive-Anatomy-Visualization

This repository is contains information and links for the publication *Multi-Layer-Gaussian-Splatting-for-Immersive-Anatomy-Visualization*.

## Code

The used code is available from multiple directories. For your convenience, they are included here as submodules:

- Unity Rendering code, at: https://github.com/roth-hex-lab/Multi-Layer-Anatomy-GS-Unity-Rendering
- GS Training code, at: https://github.com/roth-hex-lab/Multi-Layer-Anatomy-GS-Training
- Data Generation code, at: https://github.com/roth-hex-lab/Multi-Layer-Anatomy-GS-Data-Generation
- Miscellaneous scripts at: https://github.com/roth-hex-lab/Multi-Layer-Anatomy-GS-Scripts

Check out the ones you need, or clone the target repositories directly.

## Dataset and Models

Dataset, trained models and evaluation results are available from the projects OSF page here: https://osf.io/tuwh5/ / DOI 10.17605/OSF.IO/TUWH5

## Paper

**Authors:** Constantin Kleinbeck†, Hannah Schieber†, Klaus Engel‡, Ralf Gutjahr‡, Daniel Roth†

† Technical University of Munich, Clinic for Orthopedics and Sports Orthopedics, Machine Intelligence in Orthopedics

‡ Siemens Healthineers AG

Find the paper here: 

Citation:
```
in progress
```

### Abstract

In medical image visualization, path tracing of volumetric medical data like \ac{ct} scans produces lifelike three-dimensional visualizations. Immersive \ac{vr} displays can further enhance the understanding of complex anatomies. Going beyond the diagnostic quality of traditional 2D slices, they enable interactive 3D evaluation of anatomies, supporting medical education and planning. Rendering high-quality visualizations in real-time, however, is computationally intensive and impractical for compute-constrained devices like mobile headsets.

We propose a novel approach utilizing \ac{gs} to create an efficient but static intermediate representation of CT scans. We introduce a layered GS representation, incrementally including different anatomical structures while minimizing overlap and extending the GS training to remove inactive Gaussians. We further compress the created model with clustering across layers. 

Our approach achieves interactive frame rates while preserving anatomical structures, with quality adjustable to the target hardware. Compared to standard GS, our representation retains some of the explorative qualities initially enabled by immersive path tracing. Selective activation and clipping of layers are possible at rendering time, adding a degree of interactivity to otherwise static GS models. This could enable scenarios where high computational demands would otherwise prohibit using path-traced medical volumes.