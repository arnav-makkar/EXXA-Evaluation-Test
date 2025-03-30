# ALMA Autoencoder for 1250μm Continuum Observations

## Results

SSIM: 
MSE: 

## 📌 Project Overview
This project implements a convolutional autoencoder to reconstruct synthetic ALMA continuum observations (1250μm) from .fits files. The goal is to learn a compressed latent representation of astronomical images while preserving key structures.


## 🚀 Features
- Handles .fits format using astropy.io.fits.

- Autoencoder with accessible latent space for analysis.

- Quantitative metrics: Mean Squared Error (MSE) & Multiscale Structural Similarity (MS-SSIM).

- Supports high-resolution images (600×600) with deep convolutional layers.

- Visualization tools: Loss curves, reconstructed images, latent space projections.


## 🛠 Model Architecture
The autoencoder consists of:

- Encoder

    - 4 Convolutional layers (ReLU, BatchNorm, MaxPooling)

    - Fully connected latent space (128-dimension)

- Decoder

    - Transposed convolutions with upsampling

    - Sigmoid activation to match input range

## 📊 Visualization
- Reconstructed vs. Original Images

- MSE and SSIM plots over epochs

- Latent Space Visualization using t-SNE

## 🚀 Future Improvements
- Implement U-Net-based autoencoder for sharper reconstructions.

- Add self-supervised contrastive learning in the latent space.

- Train on higher resolution (1200×1200) images for ALMA-scale detail.