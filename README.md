# BENet: A Bayesian Ensemble Network Framework for Pitch Period Steganography Detection

This repository contains the official implementation of the paper "BENet: A Bayesian Ensemble Network Framework for Pitch Period Steganography Detection", submitted to *Signal Processing*.

## Abstract
Detecting Pitch Period Modulation~(PPM) steganography within compressed speech streams presents significant challenges, particularly at low embedding rates~(\textless 10\,\%) and for short-duration signals~(\textless 1\,s) where conventional methods often lack sensitivity. Existing steganalysis approaches frequently struggle under these conditions or suffer from limitations like the sensitivity-cancellation effect inherent in single Bayesian network models. This paper introduces BENet, a Bayesian Ensemble Network framework systematically constructed to enhance detection robustness and efficiency for PPM steganalysis. Guided by a Pitch Delay Spatiotemporal Model~(PDSM), BENet comprises specialized Bayesian subnetworks, each modeling a fundamental pitch-correlation pattern (self, intra-, or inter-frame). A cornerstone of BENet is its feature-level integration strategy: aggregated log-likelihood features, extracted independently from each subnetwork using standard probabilistic methods, are concatenated. These features then undergo standardization before being classified by an optimized linear Support Vector Machine. This decoupled approach, processing diverse correlation evidence before optimized classification, is designed to mitigate sensitivity cancellation and bolster overall detection performance. Furthermore, the framework incorporates Regularized Residual analysis, a proposed heuristic metric, to assess the relative statistical sensitivity of different correlation patterns to steganography, offering insights for identifying informative features and guiding potential model optimization. Comprehensive experimental evaluations demonstrate that BENet achieves high detection accuracy compared with several state-of-the-art techniques, exhibiting particularly strong advantages in challenging low-embedding-rate (\textless 10\,\%) and extremely short-duration (\textless 1\,s) scenarios. Processing speech efficiently at an average of approximately 12.87\,ms/s, BENet presents a compelling balance between high detection accuracy and computational feasibility, offering a structured and effective framework to strengthen the security of modern speech communication systems against covert channels.

## Requirements
*   Python >= 3.8
*   scikit-learn
*   numpy

## Usage
The full source code, pre-trained models, and feature extraction scripts will be released in this repository immediately upon the acceptance of the paper.

## Citation
If you find this work useful, please consider citing: To be updated
