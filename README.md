# MNIST_GANs
# GANs for Medical Image Generation

## Project Description
This project implements and compares three Generative Adversarial Network (GAN) architectures for generating synthetic chest X-ray images using the MedMNIST dataset. The implemented models include:
- LS-GAN (Least Squares GAN)
- WGAN (Wasserstein GAN)
- WGAN-GP (Wasserstein GAN with Gradient Penalty)

## Key Features
- Medical image generation using ChestMNIST dataset
- Comparative analysis of three GAN architectures
- Quantitative evaluation using Inception Score (IS) and Fréchet Inception Distance (FID)
- Training monitoring with TensorBoard
- Periodic sample generation for qualitative assessment

## Results Summary
After 50 epochs of training:
| Model    | Inception Score (↑) | FID Score (↓) |
|----------|-------------------|--------------|
| LS-GAN   | 1.0332            | 354.2737     |
| WGAN-GP  | 1.0274            | 337.1579     |
| WGAN     | **1.0261**        | **275.0643** |

*WGAN demonstrated the best performance with the lowest FID score.*

## Requirements
- Python 3.8+
- PyTorch 1.12+
- torchvision
- tensorboard
- medmnist
- numpy
- matplotlib

## Installation
```bash
git clone https://github.com/riya0785/MNIST_GANs.git
cd MNIST_GANs
pip install -r requirements.txt
jupyter notebook GANs_MedMNIST.ipynb
