# Image-Reconstruction-from-Hierarchical-Representations-of-Human-Visual-Cortex-Activities

## Introduction

Reconstructing stimuli images from brain activity has been a rising topic in the field of computational neuroscience due to the advent of deep learning algorithms and the ad-vancement in functional Magnetic Resonance Imaging (fMRI) techniques. The applica-tion of deep neural networks on larger fMRI-image-paired dataset has demonstrated sig-nificant improvement in brain decoding tasks recently. Moreover, perceptive contents be-ing hierarchically encoded in human brain has been the key to many research break-throughs in the field. This concept provides a new window into the internal mechanisms of brain system for scientists.

In this work, we follow the current state-of-the-art method “divide-and-conquer” pro-posed by Fang (2020). We are able to reproduce reconstruction results within 10% of the state-of-the-art performance. Based on the reproduced work, we further enhance our per-formance by introducing K-means image clustering method that captures more accurate semantic features for reconstructed images. Our experiments demonstrate the feasibility and flexibility of “divide-and-conquer” method in image reconstruction task. Most im-portantly, incorporating fMRI signals from different regions of visual cortex with different decoders improves the image reconstruction performance. Such implementation results map to the concept of hierarchical structure of visual cortex, giving us a medium to ex-plore more about how human brain handles visual stimuli.

## Data

### fMRI Data 
fMRI data is publicly available at [OpenNeuro](https://openneuro.org/datasets/ds001506/versions/1.3.1). This dataset is released along with the original paper Shen, Horikawa, Majima, and Kamitani (2019) Deep image reconstruction from human brain activity. PLOS Computational Biology. http://dx.doi.org/10.1371/journal.pcbi.1006633

### fMRI data extraction
To access fMRI signals from .h5 files, use this python package [bdpy](https://github.com/KamitaniLab/bdpy).


### Visual Stimuli Images
For copyright reasons, we do not make the visual images used in our experiments publicly available. You can request us to share the stimulus images at https://forms.gle/ujvA34948Xg49jdn9.

## Implementation
The “divide-and-conquer” fMRI decoding approach proposed by Fang (2020) is split into 3 stages:
(1)Shape Decoding
(2)Semantic Decoding
(3)Image Reconstruciton with GAN

Follow the ipynb files named after these three stages for model training.


## Results

![](https://i.imgur.com/oxnz0V6.png)

