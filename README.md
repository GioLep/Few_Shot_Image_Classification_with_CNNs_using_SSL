# Few-Shot Image Classification Using Convolutional Neural Networks (CNNs)
## Lepidas Georgios - Diploma Thesis Few-Shot Image Classification Using Convolutional Neural Networks (CNNs) in Python

This repository contains code and documentation for the diploma thesis titled "Ανάπτυξη Ταξινομητών με χρήση Συνελικτικών Νευρωνικών Δικτύων για Κατηγοριοποίηση με Ελάχιστα Παραδείγματα", written in Greek.

- **University**: Democritus University of Thrace (DUTH)
- **Date**: October 2022
- **Location**: Xanthi, Greece
- **Supervisor**: Ioannis Boutalis

![DUTH Logo](https://github.com/GioLep/Few_Shot_Image_Classification_with_CNNs/blob/main/images/DUTH%20Logo.png)

## Structure

- `README.md`: This file.
- `Thesis.pdf`: Full thesis document.
- `Presentation.pptx`: Presentation slides.

- `docs/`: Documentation folder.
  - `Codes_Directory_Content_Structure_Description.md`: Description of the experimental code folder structure & content.

- `codes/`: Experimental code folder.
  - `Comparison_of_Depth-Width_Impact_and_SEBlock/`: Respective experimental notebooks.
  - `Comparison_of_Self-Supervision_Impact_(VAE)/`: Respective experimental notebooks.

- `images/`: Contains images used in the documentation.
  - `DUTH_logo.png`: Logo of the Democritus University of Thrace.

- `results/`: Plot & Table results folder.
  - `Comparison 1/`: Depth comparison results.
  - `Comparison 2/`: Width & Se comparison results.
  - `Comparison 3/`: Self-Supervision impact comparison results.

## Abstract


The main purpose of this diploma thesis is to study the Few-Shot Learning concept and one of the most basic Artificial Neural Networks type, Convolutional Neural Networks (CNNs). The above terms come under the purview of Machine Learning, which is an integral part of the Artificial Intelligence field.

Few-Shot Learning constitutes one of the biggest challenges and one of the most upcoming and evolutional research fields in this domain. This is due to the structural differences between the traditional machine learning methods and the few-shot learning methods. In traditional learning methods, a huge amount of data is used for the model’s training, while in few-shot learning methods the model can learn with little or no data at all, and in that way simulate human learning.

Convolutional Neural Networks is one of the most used types of artificial neural networks, applied to a variety of tasks (such as face recognition, object detection and recognition, natural language processing, and more), with predominant use in Computer Vision applications. Their functionality is based on the mathematical operation of convolution, and they are inspired by the visual brain cells of living creatures.

The principal objective of this diploma thesis is the performance monitoring and comparison of diverse convolutional classifiers, as well as the creation and development of new models for the Few-Shot Image Classification task.

More specifically, the study is based on the Generation-0 algorithm, introduced by Jathushan Rajasegaran et al in the “Self-supervised Knowledge Distillation for Few-shot Learning” [1] research paper. The official code implementation of their work ([https://github.com/brjathu/SKD](https://github.com/brjathu/SKD)) [1] constitutes the experimental basis for this diploma thesis. Generation-0 algorithm is a method where the traditional learning is combined with the addition and solution by the model during its training of an auxiliary task where the algorithm uses Self-Supervised Learning to create the auxiliary task data. With their approach, Jathushan Rajasegaran et al. [1] achieved the creation of more powerful models for the Few-shot Image Classification task.

During this thesis implementation, a total of three comparative cases are herein made focusing on:
- the effect of the convolutional networks Resnets [31] depth to the Few-Shot Image Classification performance with the utilization of Generation-0 algorithm [1],
- the effect of the convolutional networks Resnets [31] width to the same task, as well as the exploration of the assumption that the addition of a SE block [32] to the network would boost the models’ performance, and lastly,
- the assumption that a different auxiliary Self-supervised task, specifically with the usage of a Variational Autoencoder [63], would lead to improvements to the Few-Shot Image Classification task.

## Contents

### Introduction
- Few-Shot Learning
  - The Genesis
  - Utility and Role in Artificial Intelligence
- Convolutional Neural Networks
  - History and Architectures
- Experimental Part and Generation-0 Algorithm
  - Description
  - Related Research
- Thesis Structure

### I. Theoretical Part
#### Chapter 1 Convolutional Neural Networks
1.1 Types of Learning
  - Supervised Learning
  - Unsupervised Learning
  - Reinforcement Learning
  - Self-supervised Learning
1.2 Structure and Function of Convolutional Networks
  - Structure and Layers of Convolutional Neural Networks
  - Convolution Layer and Its Function
  - Volumetric - Depth Convolution Processing
  - Pooling Layer Function
  - Batch Normalization Function
  - Dropout Layer Function
  - Useful Conclusions: Properties and Advantages
1.3 Autoencoders
  - Structure and Function
  - Types of Autoencoders

#### Chapter 2 Few-Shot Learning
2.1 The Concept of Few-Shot Learning
  - Technical Definition & General Approach to Few-Shot Learning
  - Types of Processes
  - Related Forms of Learning
  - Common Datasets
  - Mathematical Modeling of the Central Challenge of Few-Shot Learning
2.2 Categorization of Few-Shot Learning Problems
  - Focus on Data
  - Focus on Model
  - Focus on Algorithm
2.3 Applications
  - Computer Vision
  - Robotics
  - Natural Language Processing
  - Acoustic Signal Processing
  - Other Applications

### II. Experimental Part
#### Chapter 3 Presentation of Experiments
3.1 Structuring and Preparation
  - Comparisons
  - Few-Shot Categories
  - Datasets
  - Training – Experiment Details & Hyperparameters
  - Evaluation on Few-Shot Task – Test Details & Hyperparameters
3.2 Comparisons
  - Comparison 1
  - Comparison 2
  - Comparison 3
3.3 Conclusion and Future Work
  - Assessment
  - Future Endeavors

## Utilized Environment/Tools

- [Kaggle](https://www.kaggle.com/)
- [Python 3.x](https://www.python.org/)
- [PyTorch](https://pytorch.org/)
- [Weights & Biases](https://wandb.ai/site) (plots extraction)

## Datasets

The datasets used in this thesis were CIFAR-FS and FC-100. These datasets were preprocessed by the [MetaOptNet](https://github.com/kjunelee/MetaOptNet) repository. For convenience, the renamed versions of the datasets are provided by [RFS](https://github.com/WangYueFt/rfs) and can be downloaded from the following link:

- [DropBox Data Packages Link](https://www.dropbox.com/sh/6yd1ygtyc3yd981/AABVeEqzC08YQv4UZk7lNHvya?e=1&dl=0)

## Python Basis Implementations

- [Baseline - Generation-0 - Rotation Self-Supervision](https://github.com/brjathu/SKD)
- [VAE Self-Supervision](https://github.com/julianstastny/VAE-ResNet18-PyTorch)


## References


[1] Jathushan Rajasegaran et al., "Self-supervised Knowledge Distillation for Few-shot Learning", https://github.com/brjathu/SKD

[31] He, K., Zhang, X., Ren, S., & Sun, J. (2016). Deep residual learning for image recognition. In Proceedings 
of the IEEE conference on computer vision and pattern recognition (pp. 770-778). 

[32] Hu, J., Shen, L., & Sun, G. (2018). Squeeze-and-excitation networks. In Proceedings of the IEEE 
conference on computer vision and pattern recognition (pp. 7132-7141). 

[63] Kingma, D. P., & Welling, M. (2014, April). Stochastic gradient VB and the variational auto-encoder. 
In Second International Conference on Learning Representations, ICLR (Vol. 19, p. 121).


## Keywords

Data Science, Machine Learning (ML), Deep Learning(DL), Few-Shot Learning, Self-Supervised Learning, Computer Vision, Image Classification, Convolutional Neural Networks (CNNs), Artificial Neural Networks (ANNs), Autoencoders

