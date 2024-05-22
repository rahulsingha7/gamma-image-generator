# Gamma Image Generator

## Overview
This project sets up and trains a Generative Adversarial Network (GAN) using TensorFlow to generate images based on features extracted from filenames. The GAN consists of a generator that creates images from noise and specified features, and a discriminator that distinguishes real images from generated ones.

## Dataset
- **Image Source**: Images loaded from Google Drive.
- **Features**: Extracted from filenames, including velocity, feature1, and feature2.

## Preprocessing and Feature Extraction
1. **Install Libraries**: Necessary libraries are installed.
2. **Mount Google Drive**: Access images stored in Google Drive.
3. **Load and Normalize Images**: Images are loaded and normalized for processing.
4. **Extract Features**: Features such as velocity, feature1, and feature2 are extracted from filenames.
5. **Prepare TensorFlow Dataset**: Create a TensorFlow dataset with images and corresponding features.

## GAN Architecture
### Generator
- **Input**: Noise vector and features.
- **Output**: Generated image.
- **Structure**: A neural network that takes noise and features as input and outputs a generated image.

### Discriminator
- **Input**: Image (real or generated).
- **Output**: Probability of the image being real.
- **Structure**: A neural network that classifies images as real or fake.

## Training
- **Epochs**: 2000
- **Loss Functions**: Specific loss functions for the generator and discriminator.
- **Optimizers**: Specific optimizers for the generator and discriminator.
- **Checkpointing**: Saving model checkpoints during training.
- **Image Generation**: Generating and saving images at each epoch.

## Results
After training, the generator model can produce new images based on user inputs for the features. The generated images are displayed using Matplotlib.

### Visualizations
- **Generated Images Over Epochs**
 - ![Generated Images](https://i.ibb.co/PTGrhrN/gi.png)
