# Monet Style Transfer Using Generative Adversarial Networks

## Overview
This project applies Generative Adversarial Networks (GANs) for style transfer, converting real-world photos into Monet-style paintings. The model is trained on the Kaggle "GAN Getting Started" dataset, leveraging a U-Net-based generator and a deep convolutional discriminator.

## Dataset
The dataset consists of two sets of images:
- **Monet Paintings:** A collection of Monet artworks.
- **Real Photos:** Natural images intended to be transformed into Monet-style paintings.

These datasets are used to train a GAN model that learns to generate Monet-like outputs from real-world photos.

## Model Architecture
The project implements a U-Net generator and a convolutional discriminator:
- **U-Net Generator:** Designed to preserve image details while applying artistic transformations.
- **Discriminator:** A convolutional neural network that distinguishes between generated and real Monet images.

## Training
- The model is trained using an adversarial loss with an additional L1 loss to ensure content preservation.
- Label smoothing is applied to stabilize training.
- Mixed precision training is used for efficiency.

## Results
The model produces Monet-like images with varying levels of detail and artistic effects. While some images retain sharp details, others exhibit blocky artifacts or excessive smoothing, indicating potential areas for further refinement.

## Improvements and Future Work
- Experimentation with different architectures, including ResNet-based generators.
- Fine-tuning hyperparameters for improved training stability.
- Incorporating perceptual loss to enhance texture and detail retention.
- Increasing dataset diversity for more generalized results.



