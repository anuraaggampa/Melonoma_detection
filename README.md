# Melanoma Skin Cancer Detection

## Abstract
Melanoma is the deadliest form of skin cancer among over 200 types of cancer. The diagnostic process starts with clinical screening, followed by dermoscopic analysis and histopathological examination. Early-stage detection of melanoma significantly improves its curability. Dermatologists initially use high-speed cameras to capture dermatoscopic images of skin lesions, achieving 65-80% accuracy in diagnosis without additional support. When combined with visual examinations by cancer specialists, this accuracy improves to 75-84%. The goal of this project is to develop an automated classification system using image processing techniques to identify skin cancer from images of skin lesions.

## Problem Statement
The current process for diagnosing melanoma involves a skin biopsy, where a dermatologist examines a skin lesion sample under a microscope. This procedure can take over a week, from scheduling an appointment to receiving the biopsy report. This project aims to shorten this timeframe to a couple of days by developing a predictive model. The approach utilizes a Convolutional Neural Network (CNN) to classify nine types of skin cancer from images of skin lesions, potentially benefiting millions by reducing diagnosis time.

## Motivation
The primary goal is to reduce skin cancer mortality by leveraging advanced image classification technology. The motivation behind this project is to utilize the progress made in computer vision, machine learning, and deep learning to create scalable solutions that promote public health.

## CNN Architecture Design
To classify skin cancer using images of skin lesions, a custom CNN model was developed to achieve higher accuracy and better results in the classification task. The architecture includes the following components:

- **Rescaling Layer**: Normalizes input from the [0, 255] range to the [0, 1] range.
- **Convolutional Layer**: Applies convolution operations to the input, reducing image size and aggregating information.
- **Pooling Layer**: Reduces the dimensions of feature maps, decreasing the number of parameters and computation required.
- **Dropout Layer**: Randomly sets input units to zero during training to prevent overfitting.
- **Flatten Layer**: Converts data into a 1-dimensional array for input to the next layer, connecting it to a fully-connected layer.
- **Dense Layer**: A deeply connected neural network layer where each neuron receives input from all neurons of the previous layer.
- **Activation Function (ReLU)**: Outputs the input directly if positive, otherwise outputs zero, helping models learn faster and perform better.
- **Activation Function (Softmax)**: Used in the output layer to predict a multinomial probability distribution, ensuring output probabilities range between 0 and 1 and sum to one.

By integrating these components, the custom CNN model aims to accurately classify various types of skin cancer, offering a faster diagnostic alternative.