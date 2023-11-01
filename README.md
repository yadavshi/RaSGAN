## Synthesizing Iris Images Using RaSGAN With Application in Presentation Attack Detection


**iWarpGAN: Disentangling Identity and Style to Generate Synthetic Iris Images**<br>
Shivangi Yadav, Cunjian Chen and Arun Ross<br>
https://openaccess.thecvf.com/content_CVPRW_2019/papers/Biometrics/Yadav_Synthesizing_Iris_Images_Using_RaSGAN_With_Application_in_Presentation_Attack_CVPRW_2019_paper.pdf<br>

Abstract: *In this work we design a new technique for generating synthetic iris images and demonstrate its potential for presentation attack detection (PAD). The proposed technique utilizes the generative capability of a Relativistic Average Standard Generative Adversarial Network (RaSGAN) to synthesize high quality images of the iris. Unlike traditional GANs, RaSGAN enhances the generative power of the network by introducing a "relativistic" discriminator (and generator), which aims to maximize the probability that the real input data is more realistic than the synthetic data (and vice-versa, respectively). The resultant generated images are observed to be very similar to real iris images. Furthermore, we demonstrate the viability of using these synthetic images to train a PAD system that can generalize well to "unseen" attacks, i.e., the PAD system is able to detect attacks that were not used during the training phase.*


## Release notes

This repository is a Pytorch implementation of RaSGAN that utilizes features from https://github.com/AlexiaJM/RelativisticGAN/tree/master


## Requirements

* Linux and Windows are supported, but we recommend Linux for performance and compatibility reasons.
* 64-bit Python 3.8 and PyTorch 1.9.0 (or later). See https://pytorch.org for PyTorch install instructions.
* CUDA toolkit.  (Why is a separate CUDA toolkit installation required?  See [Troubleshooting](./docs/troubleshooting.md#why-is-cuda-toolkit-installation-necessary)).


## Getting started

## Training

You can train new networks using `RaSGAN.py`. For example:

```.bash
# RaSGAN model to generate images using noise as input
python RaSGAN.py --path=['./Extra/1', './Train_Data'] --input_folder=Train_Data --output_folder=Output_Folder

```



References:
1. [The relativistic discriminator: a key element missing from standard GAN](https://arxiv.org/abs/1807.00734), Jolicoeur-Martineau et al. 2017


## Citation

```
@InProceedings{Yadav_2019_CVPR_Workshops,
author = {Yadav, Shivangi and Chen, Cunjian and Ross, Arun},
title = {Synthesizing Iris Images Using RaSGAN With Application in Presentation Attack Detection},
booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) Workshops},
month = {June},
year = {2019}
}
```

## Development

This is code is under development to improve the network and its performance

