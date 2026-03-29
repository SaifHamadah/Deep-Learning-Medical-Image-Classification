# Deep-Learning-Medical-Image-Classification
Deep learning project for classifying skin disease images into 22 categories using PyTorch. Compares MLP, CNN, AlexNet, and VGG16 models with preprocessing, augmentation, and evaluation. Focuses on improving diagnostic support through automated medical image analysis.

## Project Overview
The goal of this project is to assist medical image analysis by building and evaluating multiple deep learning models for multi-class skin disease classification.

## Models Used
- MLP
- CNN
- AlexNet
- VGG16

## Tools and Technologies
- Python
- PyTorch
- Google Colab
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Dataset
Dataset used:
Skin Disease Dataset from Kaggle

Link:
https://www.kaggle.com/datasets/pacificrm/skindiseasedataset

## Preprocessing
- Image resizing to 224x224
- Normalization using ImageNet mean and standard deviation
- Stratified split into training, validation, and test sets
- Data augmentation on training data:
  - Random horizontal flip
  - Small random rotations

## Training Setup
- Loss function: CrossEntropyLoss
- Optimizer: Adam
- Learning rate: 1e-4
- Batch size: 64
- Epochs: 10
- Weight decay used in enhanced models
- Learning rate scheduler for improved training

## Results Summary

### Base Models
- CNN: Test Accuracy = 28.8%
- VGG16: Test Accuracy = 50.1%
- AlexNet: Test Accuracy = 47.5%
- MLP: Test Accuracy = 22.0%

### Enhanced Models
- CNN: Test Accuracy = 14.1%
- VGG16: Test Accuracy = 51.5%
- AlexNet: Test Accuracy = 48.4%
- MLP: Test Accuracy = 21.3%

## Key Findings
- Transfer learning models outperformed models trained from scratch.
- VGG16 achieved the best overall performance.
- MLP showed strong underfitting because it cannot capture spatial image features effectively.
- AlexNet and VGG16 showed better feature extraction and generalization.

## Repository Contents
- `notebooks/Final_Code(ALL).ipynb`: full implementation
- `reports/Final Report.docx`: final project report

## Future Improvements
- Use a larger balanced dataset
- Train for more epochs
- Apply better augmentation
- Add confusion matrix and per-class F1-score
- Try EfficientNet, ResNet, or Vision Transformers

## Author
Saif Ashraf Hamadah
