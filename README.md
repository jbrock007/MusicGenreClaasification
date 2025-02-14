# Music Genre Classification using Deep Learning

This project implements a Convolutional Neural Network (CNN) to classify music into different genres using mel spectrograms. The model can classify audio into 10 different music genres: blues, classical, country, disco, hiphop, jazz, metal, pop, reggae, and rock.

## Overview

The system works by:
1. Converting audio files into mel spectrograms
2. Splitting audio into overlapping chunks
3. Processing these chunks through a deep CNN
4. Classifying the music into one of ten genres

## Requirements

python
librosa
tensorflow
numpy
matplotlib
seaborn
sklearn
IPython

## Dataset Structure

The dataset should be organized as follows:
Data/
├── blues/
├── classical/
├── country/
├── disco/
├── hiphop/
├── jazz/
├── metal/
├── pop/
├── reggae/
└── rock/

Each folder should contain .wav files of the respective genre.

## Model Architecture

The CNN model consists of:
- Multiple Convolutional layers with increasing filters (32 → 512)
- MaxPooling layers for dimensionality reduction
- Dropout layers (0.3, 0.45) for regularization
- Dense layers for final classification
- Input shape: (150, 150, 1)
- Output: 10 classes (genres)

## Performance

The model achieves:
- Training Accuracy: ~99.5%
- Validation Accuracy: ~91.3%
- Training Loss: 0.017
- Validation Loss: 0.386

## Usage

1. **Data Preprocessing**

2. 
