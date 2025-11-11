---
layout: default
title: DSC 180A Methodology Assignment 4
---

**Name**: Jason Tran  
**Email:** jat037@ucsd.edu

**Section:** B15  
**Mentor:** Yu-Xiang Wang

## Q2 Brainstorming

**What is the most interesting topic covered in your domain this quarter?**

The emergence of training-free differential privacy (DP) through Private Evolution (PE) represents a very incredible paradigm shift in privacy-preserving machine learning. PE challenges the assumption that strong DP requires direct model training, using only black-box API calls to foundation models and achieving some pretty remarkable results. This democratizes privacy-preserving synthetic data generation and makes formal privacy guarantees accessible to normal practictioners, since we no longer need access to specialized enterprise infrastructure or model weights and gradients.

**Describe a potential investigation you would like to pursue for your Quarter 2 Project.**

We will extend our comparative analysis to Intel's structured telemetry data to investigate whether privacy-utility trade-offs observed in vision domains generalize to tabular and time-series data. This addresses the issue that most DP synthetic data work (at least in academia) focuses on modalities related to images, while the industry predominantly involves structured data with mixed feature types, temporal dependencies, and high dimensionality. We aim to evaluate both methods on this industry data, assessing scalability and whether PE's advantages remain tempting even when foundation models for structured data are less mature technologies than vision models.

**What is a potential change you'd make to the approach taken in your current Quarter 1 Project?**

We would implement more comprehensive evaluation metrics beyond FID. Additionally, we could explore adaptive privacy budget allocation across PE's iterative selection process, which may improve utility while preserving the same epsilon.

**What other techniques would you be interested in using in your project?**

Several complementary techniques could strengthen our analysis, like PATE (Private Aggregation of Teacher Ensembles) as an alternative DP paradigm using knowledge distillation, DP-GAN methods for comparison, etc. We could also take a look at privacy amplification by subsampling, and formally analyzing how batch sampling in DP-SGD affects the tradeoff between privacy and utility.
