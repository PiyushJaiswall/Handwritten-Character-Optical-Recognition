# Handwritten Character Optical Recognition

![OCR](https://img.shields.io/badge/OCR-Handwritten%20Recognition-blue.svg)
![Python](https://img.shields.io/badge/Python-3.8%2B-brightgreen.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

This repository contains the code, report, and model for an Optical Character Recognition (OCR) system focused on handwritten characters.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Usage](#usage)
- [Results](#results)
- [Conclusion](#conclusion)
- [Acknowledgements](#acknowledgements)
- [References](#references)

## Introduction

Optical Character Recognition (OCR) is a technology that converts different types of documents, such as scanned paper documents, PDF files, or images captured by a digital camera, into editable and searchable data. This project aims to develop an OCR system for handwritten characters using deep learning techniques.

## Dataset

The dataset used for training the OCR model consists of images containing handwritten text and their corresponding labels. The images are preprocessed and augmented to enhance the performance of the model.

### Preprocessing

- **Grayscale Conversion**: Convert images to grayscale.
- **Normalization**: Scale pixel values to the range [0, 1].
- **Resizing**: Uniformly resize images to a fixed dimension.

### Data Augmentation

- **Rotation**: Randomly rotate images.
- **Zoom**: Apply random zoom to images.
- **Shift**: Apply random horizontal and vertical shifts.

## Model Architecture

The OCR model is built using a combination of Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs) to recognize and interpret text in images.

### Convolutional Layers

- Extract spatial features from input images.

### Recurrent Layers

- Long Short-Term Memory (LSTM) or Gated Recurrent Unit (GRU) layers to capture sequential dependencies.

### Fully Connected Layers

- Perform classification based on extracted features.

## Training

The model is trained using the preprocessed and augmented dataset with the following steps:

1. **Data Augmentation**: Enhancing the dataset by applying various transformations.
2. **Model Compilation**: Configuring the model with appropriate loss functions and optimizers.
3. **Model Training**: Training the model using the augmented dataset.

## Evaluation

The trained model is evaluated on a separate test set to measure its accuracy and performance. Various metrics such as accuracy, precision, recall, and F1-score are used for evaluation.

### Metrics

- **Accuracy**: Proportion of correct predictions.
- **Precision**: Proportion of true positive predictions.
- **Recall**: Proportion of actual positives correctly identified.
- **F1-Score**: Harmonic mean of precision and recall.

## Usage

To use the OCR model, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/PiyushJaiswall/Handwritten-Character-Optical-Recognition.git
    cd Handwritten-Character-Optical-Recognition
    ```

2. Install the required dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Load the trained model and run the OCR on your images:
    ```python
    from keras.models import load_model
    model = load_model('model1.h5')
    # Load and preprocess your image
    # Run the OCR
    ```

## Results

The results of the OCR model, including accuracy and performance metrics, are detailed in the project report (`final_report.pdf`).

### Example Results

| Image | Predicted Text |
|-------|----------------|
| ![Example 1](images/example1.png) | `Hello` |
| ![Example 2](images/example2.png) | `World` |

## Conclusion

This project demonstrates the development and implementation of an OCR system using deep learning techniques. The model shows promising results in recognizing and interpreting handwritten text from images.

## Acknowledgements

We would like to thank our mentors and peers for their guidance and support throughout this project.

## References

- [Keras Documentation](https://keras.io/)
- [Deep Learning with Python](https://www.manning.com/books/deep-learning-with-python)
- [Handwritten Character Recognition Dataset](https://www.kaggle.com/datasets/)

---

### Repository Structure


For any questions or suggestions, please feel free to open an issue or contact us.

[![GitHub Issues](https://img.shields.io/github/issues/PiyushJaiswall/Handwritten-Character-Optical-Recognition.svg)](https://github.com/PiyushJaiswall/Handwritten-Character-Optical-Recognition/issues)
[![GitHub Stars](https://img.shields.io/github/stars/PiyushJaiswall/Handwritten-Character-Optical-Recognition.svg)](https://github.com/PiyushJaiswall/Handwritten-Character-Optical-Recognition/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/PiyushJaiswall/Handwritten-Character-Optical-Recognition.svg)](https://github.com/PiyushJaiswall/Handwritten-Character-Optical-Recognition/network)
