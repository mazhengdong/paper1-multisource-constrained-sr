# Deep Learning–based Multi-source Constrained Image Super-Resolution (Paper 1)

This repository corresponds to a **first-author research paper** on **deep learning–based multi-source image super-resolution**, with an emphasis on **multi-source constraint modeling** to improve fine-scale reconstruction accuracy and spatial consistency.

## Overview

Reconstructing high-resolution images from coarse-resolution observations is a critical yet challenging task due to scale mismatch, information loss, and strong spatial heterogeneity. This work proposes a **multi-source constrained deep learning framework** that integrates heterogeneous auxiliary variables into a unified super-resolution model, enabling more accurate and physically consistent fine-scale reconstruction.

## Dataset

* Multi-source geospatial datasets
* Combination of primary low-resolution images and auxiliary constraint variables
* Target resolution: coarse (~10–25 km) → fine (~500 m)
* Independent temporal periods for training and evaluation

> Note: Due to data licensing and policy restrictions, the original datasets are not publicly released.

## Method

* End-to-end deep neural network for image super-resolution
* Explicit modeling of multi-source auxiliary constraints
* Multi-scale feature extraction to capture spatial heterogeneity
* Feature fusion strategy for combining primary inputs and constraint variables
* Reconstruction-oriented loss functions for stable training

## Experiments

* Ablation experiments on different constraint-variable combinations
* Sensitivity analysis across spatial and temporal subsets
* Quantitative evaluation using accuracy-based and error-based metrics
* Spatial pattern analysis to assess reconstruction realism

## Implementation

The PyTorch implementation of the core model architecture and training pipeline is shared in the following repository:

* **Core implementation**: [https://github.com/mazhengdong/dl-multisource-super-resolution-core.git](https://github.com/mazhengdong/dl-multisource-super-resolution-core.git)

This repository focuses on **project-level experimental configuration, constraint design, and result analysis** corresponding to Paper 1.

## Results

Experimental results demonstrate that incorporating multi-source constraints significantly enhances super-resolution performance compared with unconstrained or single-source baselines, particularly in regions with complex spatial variability.

## Author

* **First Author & Core Algorithm Developer**: Mazhengdong

## Citation

If you find this work useful, please cite the corresponding paper.

