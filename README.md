# AutoEncoder for MNIST Dataset

This repository contains an implementation of an AutoEncoder neural network using Keras for the MNIST dataset. The AutoEncoder takes 28x28 pixel images as input, encodes them into a lower-dimensional representation (16x16 pixels), and then decodes them back to the original size. Additionally, denoising of the decoded images has been implemented to enhance human readability.

## Getting Started

To get started with this project, you can follow these steps:

1. Clone the repository to your local machine:

git clone https://github.com/kroax9797/AutoEncoder.git

2. Install the required dependencies:
pip install -r requirements.txt

## Implementation Details
### Dataset
The MNIST dataset consists of grayscale images of handwritten digits (0-9), each of size 28x28 pixels. The dataset is split into a training set and a test set.

### Model Architecture
The AutoEncoder architecture consists of an encoder and a decoder. Both encoder and decoder are neural networks with several layers. The encoder compresses the input images into a lower-dimensional representation, and the decoder reconstructs the original images from this representation.

### Training
The AutoEncoder is trained on the training set of the MNIST dataset. The loss function used during training is chosen(binary crossentropy) to minimize the reconstruction error between the original and reconstructed images. In this implementation .

## Denoising
To improve the clarity of the reconstructed images, a denoising step is applied after decoding. This helps in removing noise and enhancing the visual quality of the images. The denoiser is also trained indegeniously by having noisy dataset created by adding noise to the dataset available and training on it . By giving noisy dataset as input and the orignal data as the output .

## Results
After training the AutoEncoder, the model is evaluated on the test set. Sample input images are encoded, decoded, and denoised to showcase the effectiveness of the AutoEncoder in reconstructing handwritten digits.

## Acknowledgments
The code in this repository is based on the concepts learned from various sources, including online tutorials, books, and research papers.

### Tejas Mhaiskar
