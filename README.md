# PCA and Image Compression/Decompression
This repository contains three Jupyter Notebooks that explore Principal Component Analysis (PCA) for image compression and decompression tasks.

## Notebook 1: PCA for MNIST Digits
### Functionality:
  - Loads an image (digit) from the MNIST dataset.
  - Implements image pre-processing (normalization).
  - Defines a `PCA` class for eigenvector and eigenvalue calculation, compression, and reconstruction.
  - Compresses the image using a specified number of components.
  - Reconstructs the image from the compressed representation.
  - Visualizes the original, compressed, and reconstructed images.

## Notebook 2: PCA for Face Recognition with SVM

### Data:
  - Utilizes the Labeled Faces in the Wild (LFW) dataset for face recognition.
  - Splits the data into training and testing sets.

### PCA:
  - Implements a `PCA` class similar to Notebook 1.
  - Compresses the face images using PCA.
  - Calculates the mean face for both original and decompressed images.

### Face Recognition:
  - Trains an SVM classifier on the compressed training data and face labels.
  - Evaluates the accuracy of the SVM classifier on compressed data.
  - Compares the accuracy with an SVM classifier trained on the original (uncompressed) data.

## Notebook 3: PCA for Color Image Compression

### Functionality:
  - Loads a color image (e.g., 'moon.png').
  - Splits the image into red, green, and blue channels.
  - Calculates the mean and covariance matrix for each channel.
  - Computes the eigenvalues and eigenvectors for each channel's covariance matrix.
  - Selects a specified number of top principal components (PCs) for compression.
  - Transforms each channel data to the principal component space.
  - Merges the transformed channels and saves the compressed image.
  - Reconstructs the image by projecting back from the principal component space and merging channels.
  - Saves the reconstructed image.
  - Visualizes both the compressed and reconstructed images.
