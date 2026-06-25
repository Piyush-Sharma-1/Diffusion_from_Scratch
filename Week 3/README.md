# Week 3 – Variational Autoencoder (VAE)

## Overview

This week focused on implementing a Variational Autoencoder (VAE) from scratch using PyTorch. The objective was to apply the concepts learned in Weeks 1 and 2 by building a generative model capable of learning a latent representation of data and generating new samples.

## Topics Studied

- Variational Autoencoders (VAEs)
- Encoder-Decoder Architecture
- Latent Space Learning
- Reparameterization Trick
- Reconstruction Loss
- KL Divergence Regularization
- VAE Training using ELBO

## Implementation Details

### Dataset
- Two-Moons dataset generated using Scikit-Learn.
- Data loaded using PyTorch DataLoader.

### Encoder
- Maps input data into latent distribution parameters.
- Outputs:
  - Mean (μ)
  - Log Variance (logσ²)

### Reparameterization Trick
- Implemented stochastic sampling using:

z = μ + σ × ε

where ε is sampled from a standard Gaussian distribution.

### Decoder
- Reconstructs input samples from latent representations.
- Learns meaningful compressed representations of the dataset.

### Loss Function

Implemented VAE Loss:

Loss = Reconstruction Loss + β × KL Divergence

Components:
- Reconstruction Loss (MSE Loss)
- KL Divergence Regularization
- β-VAE formulation with β = 0.1

## Results

### Training Performance
- Successfully trained the VAE for 200 epochs.
- Training loss decreased steadily throughout training.

### Reconstruction Quality
- Reconstructed samples preserved the overall structure of the original Two-Moons dataset.

### Latent Space Visualization
- Learned meaningful latent representations.
- Similar samples were mapped to nearby regions in latent space.

### Sample Generation
- Generated new samples by sampling random points from latent space.
- Generated points followed the overall distribution of the training data.

## Key Learnings

- Understood the complete VAE pipeline.
- Implemented the reparameterization trick in PyTorch.
- Learned how KL divergence regularizes latent representations.
- Visualized latent spaces and generative sampling.
- Connected ELBO theory from Week 2 to practical implementation.

## Deliverables

- Implemented a Linear VAE from scratch.
- Trained on the Two-Moons dataset.
- Visualized:
  - Training Loss Curve
  - Reconstruction Results
  - Latent Space
  - Generated Samples

## Outcome

Successfully built and trained a Variational Autoencoder capable of learning meaningful latent representations and generating realistic samples from unseen latent vectors.
