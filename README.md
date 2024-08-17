# GAN for Generating Realistic Fake Images

## Objective

The objective of this project is to develop a Generative Adversarial Network (GAN) that can generate realistic fake images based on the source data.

## Data Preparation

The data used in this project underwent the following preprocessing steps to ensure optimal training conditions for the GAN:

- **Resized:** All images were resized to ensure uniform input dimensions.
- **Center-cropped:** Images were center-cropped to focus on the main subject and remove unnecessary borders.
- **Normalized:** Pixel values were normalized to scale them between -1 and 1, which is essential for stabilizing and improving the training process.

## Dataset

The dataset used for this project is the [Anime Face Dataset](https://www.kaggle.com/splcher/animefacedataset) available on Kaggle. This dataset contains various anime face images suitable for training the GAN.

## Model Architecture

The GAN network consists of two main components:

- **Generator:** This model generates fake images from random noise using a series of convolutional layers.
- **Discriminator:** This model, also built with convolutional layers, distinguishes between real and generated images.

## Training

The model was implemented using PyTorch and trained for 25 epochs. Throughout the training process, the generator learned to produce realistic fake images that closely resemble the source data, while the discriminator improved its ability to distinguish between real and fake images.

## Results

After 25 epochs of training, the GAN successfully generated realistic fake images. The model's performance can be further improved with additional training and fine-tuning.

## Installation

To run this project, you'll need to install the following dependencies:

```bash
pip install torch torchvision numpy matplotlib
