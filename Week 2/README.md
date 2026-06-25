# Week 2 – Deriving the VAE Loss (ELBO)

## Overview

This week focused on understanding the mathematical foundation of Variational Autoencoders (VAEs). The primary objective was to derive the Evidence Lower Bound (ELBO), which serves as the training objective for VAEs.

## Topics Studied

- Evidence Lower Bound (ELBO)
- Latent Variable Models
- Variational Inference
- Encoder and Decoder Framework
- Reconstruction Loss
- KL Divergence Regularization
- VAE Objective Function

## Key Learnings

### Variational Inference
- Learned how complex probability distributions can be approximated using simpler distributions.
- Understood the motivation behind introducing latent variables.

### Evidence Lower Bound (ELBO)
- Derived the ELBO formulation step-by-step.
- Understood why maximizing ELBO is equivalent to improving the model's ability to represent data.

### Reconstruction Loss
- Learned how reconstruction loss measures the quality of reconstructed samples.
- Understood its role in preserving information from input data.

### KL Divergence Term
- Studied how KL divergence regularizes the latent space.
- Learned why the latent distribution is encouraged to match a standard Gaussian distribution.

### VAE Loss Function

The VAE objective consists of:

Loss = Reconstruction Loss + β × KL Divergence

where:
- Reconstruction Loss ensures accurate reconstruction of input data.
- KL Divergence regularizes the latent space.
- β controls the trade-off between reconstruction quality and latent space structure.

## Outcome

Developed a mathematical understanding of the VAE training objective and gained intuition about how reconstruction loss and KL divergence work together to create meaningful latent representations.

## Deliverables

- Derived ELBO formulation.
- Studied the mathematical foundations required for implementing a Variational Autoencoder in Week 3.
