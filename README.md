# CIFAR-10 Image Classification with PyTorch

## Overview

This repository contains a comprehensive deep learning project for image classification on the CIFAR-10 dataset using PyTorch. The project explores and compares multiple machine learning and deep learning architectures, including Logistic Regression, Multi-Layer Perceptrons (MLP), Convolutional Neural Networks (CNN), Transfer Learning with AlexNet, and Adversarial Attack analysis using FGSM.

The goal is to evaluate model performance, understand the impact of architectural choices, and analyze model robustness against adversarial examples.

---

## Dataset

The project uses the CIFAR-10 dataset, which consists of:

- 60,000 color images
- 10 object classes
- Image size: 32 × 32 pixels
- 50,000 training images
- 10,000 test images

### Classes

- Airplane
- Automobile
- Bird
- Cat
- Deer
- Dog
- Frog
- Horse
- Ship
- Truck

---

## Project Objectives

- Implement baseline image classification models
- Compare performance across different architectures
- Apply transfer learning using pretrained networks
- Fine-tune deep learning models for improved accuracy
- Evaluate model robustness using adversarial attacks
- Visualize training and validation performance

---

## Models Implemented

### 1. Logistic Regression

- Baseline model using flattened image inputs
- Cross-entropy loss function
- SGD optimizer

### 2. Multi-Layer Perceptron (MLP)

- Fully connected neural network
- Hidden layers with ReLU activation
- Dropout regularization

### 3. Convolutional Neural Network (CNN)

- Multiple convolutional layers
- Max pooling layers
- Batch normalization
- ReLU activations

### 4. Transfer Learning with AlexNet

- Pretrained AlexNet feature extractor
- Modified classifier layers
- Frozen convolutional backbone

### 5. Fine-Tuned AlexNet

- Partial layer unfreezing
- End-to-end optimization
- Improved feature learning

### 6. FGSM Adversarial Attack

- Fast Gradient Sign Method implementation
- Adversarial image generation
- Model robustness evaluation

---

## Technologies Used

- Python
- PyTorch
- Torchvision
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---

## Project Structure

```text
├── CIFAR10_Project.ipynb
├── README.md
├── models/
├── results/
├── figures/
└── requirements.txt
```

---

## Training Pipeline

1. Load CIFAR-10 dataset
2. Apply image preprocessing and normalization
3. Train Logistic Regression baseline
4. Train MLP model
5. Train CNN architecture
6. Apply Transfer Learning using AlexNet
7. Fine-tune pretrained model
8. Evaluate on test dataset
9. Generate confusion matrices and performance metrics
10. Perform FGSM adversarial attack analysis

---

## Results Summary

| Model | Test Accuracy |
|---------|--------------|
| Logistic Regression | ~45% |
| MLP | ~60% |
| CNN | ~86% |
| AlexNet Transfer Learning | ~89% |
| Fine-Tuned AlexNet | **91.26%** |

---

## Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Training Loss
- Validation Loss

---

## Adversarial Robustness Analysis

The project implements the Fast Gradient Sign Method (FGSM) to:

- Generate adversarial examples
- Evaluate model vulnerability
- Compare predictions before and after perturbation
- Visualize attack effectiveness

---

## Key Learnings

- CNNs significantly outperform traditional machine learning approaches for image classification tasks.
- Transfer learning improves model performance while reducing training time.
- Fine-tuning pretrained networks yields the highest accuracy.
- Deep learning models remain vulnerable to adversarial attacks.
- Proper regularization and optimization improve generalization performance.

---

## Future Enhancements

- Implement ResNet50 and EfficientNet architectures
- Apply advanced data augmentation techniques
- Perform hyperparameter optimization
- Explore ensemble learning methods
- Implement adversarial training for improved robustness

---

## Author

**Raghu Ram Reddy Thirumala**

- M.S. in Data Science, University at Albany
- Python Developer
- Machine Learning Engineer
- Deep Learning Enthusiast

---

## License

This project is intended for educational and research purposes.
