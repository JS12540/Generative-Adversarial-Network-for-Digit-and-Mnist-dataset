# Generative-Adversarial-Network-for-Digit-and-Mnist-dataset

This repository contains code for training a GAN (Generative Adversarial Network) on a dataset. The GAN consists of a generator and a discriminator, and it aims to generate realistic samples.

## Training Parameters

- **Epochs:** 200
- **Batch Size:** 100
- **Steps per Epoch:** 500
- **Noise Size:** 50

## Training Process

The GAN is trained over 200 epochs, with updates occurring every 10 epochs. During each epoch, the generator is evaluated, and the progress is visualized.

### Discriminator Training

The discriminator is trained on batches of both real and fake samples. The goal is for the discriminator to correctly classify real samples as real (label 1) and fake samples as fake (label 0).

### Generator Training

The generator is trained to produce samples that can fool the discriminator. The discriminator is temporarily set to believe that generated samples are real (label 1), and the generator is updated based on the discriminator's feedback.

## Results

The training progress is monitored, and the losses of both the discriminator and the generator are recorded. Here are some examples:

```plaintext
Epoch: 197, Step: 450, D-Loss: 0.615, D-Acc: 65.000, G-Loss: 0.965
Epoch: 198, Step: 0, D-Loss: 0.641, D-Acc: 66.000, G-Loss: 0.987
...
Epoch: 199, Step: 450, D-Loss: 0.593, D-Acc: 65.000, G-Loss: 0.944

## Visualization
Every 10 epochs, the generated samples are visualized using the show_generator_results function.

## Dependencies
Ensure you have the necessary dependencies installed. You can find them in the requirements.txt file.

## How to Use
Clone the repository.
Install dependencies with pip install -r requirements.txt.
Run the GAN training script.
Feel free to customize the code and parameters based on your dataset and requirements.
