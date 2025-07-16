Applied Machine Learning - University of Bologna Master in Bioinformatics - 2024/2025

In this project I will evaluate the performance of both traditional Machine Learning and Deep Learning based methods on pathology image classification. I will focus the attention on four traditional ML models (Extreme Gradient Boosting, K-nearest neighbors, Support Vector Classifier and a soft voting ensemble of all the previous) and compare their performance with a fairly simple Convolutional Neural Network.

For this purpose, I opted for the MedMNIST PathMNIST dataset. MedMNIST is a large-scale, lightweight benchmark dataset collection designed for evaluating machine learning algorithms on biomedical image classification tasks. PathMNIST is a subset of MedMNIST based on colorectal cancer histology images from the DigestPath dataset. It contains 107,180 RGB images from 9 tissue classes.

A simple data augmentation routine on the training dataset will be performed to increase the samples of the less represented classes. For this task, I will use the Albumentations library to apply a randomized combination of transformations such as rotation, flipping, noise addition, blurring, affine transformations, and color adjustments.

Quantitative features will be extracted from histology images by combining color statistics and texture descriptors. Color features (mean, standard deviation, skewness, kurtosis) are computed from each RGB channel to capture staining variations. Texture is characterized using Haralick features (global structure), Local Binary Patterns (local micro-texture), and Gabor filters (frequency and orientation). Together, these features provide a comprehensive description of tissue morphology, enhancing the accuracy of image-based histopathological classification.
