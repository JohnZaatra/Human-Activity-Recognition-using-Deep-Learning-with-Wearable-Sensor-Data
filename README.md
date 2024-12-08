# Human Activity Recognition (HAR) with Wearable Sensors

## Overview

This repository showcases a comprehensive machine learning project aimed at solving the Human Activity Recognition (HAR) problem. Using data collected from wearable sensors, the goal is to accurately classify human activities such as walking, running, sitting, and standing based on acceleration data. This project demonstrates the application of several machine learning algorithms, including **Random Forest**, **CNN**, and **LSTM**, with a focus on preprocessing, model optimization, and leveraging advanced techniques like **masked autoencoders** for pretraining.

## Key Features

- **Multiple Machine Learning Models**: Implementation of **Random Forest**, **CNN**, and **LSTM** for activity classification.
- **Data Preprocessing**: Noise filtering, normalization, and segmentation of time-series data.
- **Hyperparameter Tuning**: Systematic tuning of model architectures and hyperparameters for optimal performance.
- **Masked Autoencoder**: Use of masked autoencoder pretraining to enhance model robustness and performance.
- **State-of-the-Art Techniques**: Experimentation with innovative padding algorithms and computational efficiency improvements.

## Objective

The primary goal of this project is to develop a model capable of classifying human activities accurately based on acceleration data. The models were optimized through systematic experimentation, including:

- **Preprocessing**: Noise removal, normalization, and segmentation to prepare the data for model training.
- **Model Development**: Designing deep learning architectures and exploring hyperparameters to maximize performance.
- **Evaluation**: Using accuracy, precision, recall, and F1-score to assess model performance, with a focus on real-world applicability.

## Results

### Random Forest Model:
- **Before Improvements**:
  - **Train Accuracy**: 1.0
  - **Validation Accuracy**: 0.971
- **After Improvements**:
  - **Train Accuracy**: 1.0
  - **Validation Accuracy**: 0.934

### CNN Model:
- **Before Improvements**:
  - **Training Accuracy**: 93.83%
  - **Validation Accuracy**: 89.18%
- **After Improvements**:
  - **Training Accuracy**: 83.12%
  - **Validation Accuracy**: 79.50%

### LSTM Model:
- **Before Improvements**:
  - **Training Accuracy**: 69.65%
  - **Validation Accuracy**: 67.79%
- **After Improvements**:
  - **Training Accuracy**: 81.51%
  - **Validation Accuracy**: 76.62%

### Key Improvements:
- **Model Architecture Refinement**: Explored various layer configurations, neurons, and activation functions to optimize performance.
- **Hyperparameter Tuning**: Iterative adjustments to learning rate, batch size, dropout rate, and other hyperparameters.
- **Padding Techniques**: Compared zero-padding and data-preserving padding to handle variable sequence lengths in time-series data.
- **Masked Autoencoder Pretraining**: Enhanced the model’s performance by pretraining with a masked autoencoder to capture long-term dependencies and improve generalization.

## Dataset

The dataset used for this project contains acceleration data collected from wearable sensors. It includes time-series measurements of human activity, where each activity is labeled for classification purposes.

### Files:
- `train.csv`: Training set with labels.
- `metaData.csv`: Supplemental metadata for understanding the data.
- `sample_submission.csv`: Template for submission.

### Data Columns:
- **Measurement Type**: Acceleration data in terms of `x`, `y`, and `z` coordinates.
- **Type #1**: Columns include `measurement type`, `x`, `y`, and `z` (use only rows with `measurement type = "acceleration [m/s/s]"`).
- **Type #2**: Columns include `x [m]`, `y [m]`, and `z [m]` (use all available data).

## Installation and Setup

To get started with this project, follow the steps below:

### 1. Clone the repository:
```bash
git clone https://github.com/yourusername/Human-Activity-Recognition.git
cd Human-Activity-Recognition
```
### 2. Install the required dependencies:
```bash
pip install -r requirements.txt
```

### 3. 3. Run the model:
```bash
python main.py
```

## How to Contribute

I welcome contributions to this project. If you have ideas for improvements, optimizations, or new features, feel free to fork the repository and submit a pull request. Please ensure that you follow the coding standards and include tests where applicable.

## Acknowledgments

This project is part of a broader exploration into Human Activity Recognition, where we applied state-of-the-art techniques in machine learning to a practical, real-world problem. Special thanks to the original dataset creators and the academic community for sharing valuable insights on time-series classification.

## Conclusion

This project illustrates the powerful intersection of machine learning and wearable technology in the field of Human Activity Recognition. By exploring multiple models, optimizing their performance, and experimenting with novel techniques such as masked autoencoders, the project showcases an in-depth understanding of time-series data and model refinement. I am confident that the skills developed in this project will be directly applicable to real-world challenges in data science and machine learning.

Thank you for exploring this project!

