🇰🇭 Khmer Handwritten Digit Recognition using CNN
### Overview

Handwritten digit recognition has advanced significantly since Yann LeCun’s pioneering work on the MNIST dataset in 1994. While Arabic numeral recognition has been widely studied and achieves high accuracy using Convolutional Neural Networks (CNNs), Khmer numeral recognition has received much less attention.

This project focuses on recognizing Khmer handwritten numerals (0–9) using CNN models. We create a custom dataset containing 3,000 Khmer digit images and evaluate CNN performance. The model achieved approximately 97% accuracy, demonstrating that CNN architectures can successfully recognize Khmer digits.

### Objectives

Create a Khmer handwritten numeral dataset (digits 0–9)

Preprocess images into 28×28 grayscale format

Train a CNN model to classify Khmer digits

Evaluate model performance using accuracy and loss

Support future development of Khmer AI learning tools

### Dataset Description

This project uses a self-created dataset with 10 digit classes (0–9) and a total of 3,000 images.

Dataset Types

* Digital Drawing Dataset

1,500 images

Size: 64×64×4

* Paper Drawing Dataset

1,500 images

Original size: ~800×800 pixels

Cropped to 100–400 pixels before resizing to avoid feature loss

Converted to grayscale and inverted to match digital image format

### Preprocessing Steps

The dataset is preprocessed to ensure consistency and reduce computational cost.

Steps include:

Convert image to grayscale

Resize to 28×28 pixels

Normalize pixel values to range [0,1]

Shuffle dataset for training consistency

Paper images are additionally processed using pixel inversion after grayscale conversion to reduce differences between digital and paper drawings.

### Model

This project uses a Convolutional Neural Network (CNN).

Input: 28×28 grayscale image

Output: 10 classes (digits 0–9)

Softmax activation is used to generate probability distribution for predictions

### Results

The CNN model performs well on the Khmer handwritten digit dataset.

Accuracy achieved: ~97%

Training and validation accuracy stabilize after around 30 epochs

Loss decreases quickly and remains stable close to 0

These results show that CNN models can generalize effectively for Khmer digit recognition.

### Testing

A separate testing dataset was created containing 200 images:

20 images per digit class

100 digital drawings

100 paper drawings

The model achieved strong prediction performance on both types of test images.

### File Included

This repository contains only one main file:

📌 Notebook.ipynb

Includes dataset loading

preprocessing

CNN model training

evaluation and visualization

### How to Run

Download or clone this repository

Open the notebook using Jupyter Notebook or Google Colab

Run in Jupyter Notebook
jupyter notebook


Then open:

Notebook.ipynb

⚠️ Limitations

Can recognize only one digit at a time

Cannot generalize to image types not included in training data

Cannot detect stroke direction or drawing order

### Future Work

Expand dataset size and diversity

Improve model performance using hyperparameter tuning

Support multi-digit recognition (e.g., 12, 105)

Build a kid-friendly Khmer learning application

Extend into Khmer OCR and Khmer AI chatbot tools

### License

This project is for educational and research purposes.
