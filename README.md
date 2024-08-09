# Wasserstein GAN Implementation

## Overview

Developed a Generative Adversarial Network (GAN) with a Wasserstein loss function, implementing both the generator and the critic using PyTorch to generate realistic images from random noise.

The training consists of two steps: (1) Updating discriminators for n_critic steps (such that we have an optimal critic): here we use an aggregation of three loss functions, (a) The real loss (the output scalar of the critic for real images); (b) The fake loss (same value for fake images); (c) The gradient penalty. (2) Updating generators by only considering the fake loss (to fool the critic).

![image](https://github.com/user-attachments/assets/08b83084-2bd6-4c0d-b48c-27940b5e154d)

## Generated Images 

![image](https://github.com/user-attachments/assets/f9591718-0be9-4f01-82e6-a4c93e451e5b)


