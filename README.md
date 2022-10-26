# cnn-vs-vit
This is our paper presentation for DS 5899 - Transformers. The topic of discussion: Do Vision Transformers see like Convolution Neural Networks?

[Our Presentation Slides](https://docs.google.com/presentation/d/1NSiqBuMzJEszaGAs3XfNuMyi_4NkqIEVPTo7G4usgJk/edit?usp=sharing)

## Overview

Computer Vision is a domain that focuses on the usage of deep learning algorithms to understand images. It works by transforming an image into a numerical representation (often a matrix). This matrix is ran through different mathematical functions geared towards providing a label on the image.

## Paper review

[Video recording](https://www.youtube.com/watch?v=IffBFXTnjqk&t=50s)

> Representation similarity between lower and higher layers
> - Compared with CNN, ViT has a more uniform internal representation structure (Higher similarity between lower/higher layers)

> Global & Local spatial information at lower layers 
> - CNN convolves local spatial information by convolution filter at lower layer
> - ViT incorporates global spatial information at lower layer (but also local spatial information is important)

> More spatial information is preserved in ViT than CNN

> Effects of skip connections on performance & representation similarity
> - Skip-connections impact more in ViT than in CNN (ResNets)

> Effects of dataset scale on transfer learning
> - ViT can learn high quality intermediate representations

> Connections to new architectures such as the MLP-Mixer
> - MLP-Mixer is similar to ViT rather than ResNet



## CNN vs ViT

An experiment was conducted by us to see the differences in performance between ViT and Resnet-50 when it comes to making inferences on images. 

> For our experiment:
> - The food data on Huggingface was loaded into our Jupyter Notebook file
> - We proceeded to transform the images in the data to be suitable for model training 
> - Then, we trained either ViT and Resnet on the training sets of the images
> - Finally, we evaluated the performance of both trained models on the test data


![image](https://user-images.githubusercontent.com/89406404/197955058-5f907bd6-75e5-4c9a-8695-66cd3da42a59.png)


## Summary

> ViT has created a new pathway for learning from image data via Attention

> ViT differs heavily from CNNs in terms of its ability to recognize object

> - It views images uniformly across all layers

> ViT needs to have been pre-trained on a lot of data before it can go on to clearly outperform CNNs


## References

[Do Vision Transformers See Like Convolution Neural Networks?](https://arxiv.org/abs/2108.08810)

[Vision Transformer for Image Classification](https://www.youtube.com/watch?v=HZ4j_U3FC94)

[A Comprehensive Guide to Convolutional Neural Networks — the ELI5 way](https://towardsdatascience.com/a-comprehensive-guide-to-convolutional-neural-networks-the-eli5-way-3bd2b1164a53)

[Attention augmented convolutional networks.](https://arxiv.org/abs/1904.09925)

[MLP-Mixer: An all-MLP Architecture for Vision](https://arxiv.org/abs/2105.01601)
