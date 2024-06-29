# Few_Shot_Image_Classification_with_CNNs
Lepidas Georgios - Diploma Thesis on Few Shot Image Classification with CNNs in Python

This repository contains code and documentation for the diploma thesis titled "Ανάπτυξη Ταξινομητών με χρήση Συνελικτικών Νευρωνικών Δικτύων για Κατηγοριοποίηση με Ελάχιστα Παραδείγματα", written in Greek.

- **University**: Democritus University of Thrace (DUTH)
- **Date**: October 2022
- **Location**: Xanthi, Greece
- **Supervisor**: Yannis Boutalis

![DUTH Logo](https://github.com/GioLep/Few_Shot_Image_Classification_with_CNNs/blob/main/images/DUTH%20Logo.png)

## Structure

- `README.md`: This file.
- `Thesis.pdf`: Full thesis document.
- `Presentation.pptx`: Presentation slides.

- `docs/`: Documentation folder.
  - `Codes_Directory_Content_Structure_Description.md`: Detailed description of the experimental code.

- `codes/`: Experimental code folder.
  - `Comparison_of_Depth-Width_Impact_and_SEBlock/`: Respective experimental notebooks.
  - `Comparison_of_Self-Supervision_Impact_(VAE)/`: Respective experimental notebooks.

- `images/`: Contains images used in the documentation.
  - `DUTH_logo.png`: Logo of the Democritus University of Thrace.

- `results/`: Plot results folder.
  - `Comparison 1/`: Depth comparison plot results.
  - `Comparison 2/`: Width & Se comparison plot results.
  - `Comparison 3/`: Self-Supervision impact comparison plot results.

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


## Thesis Structure

## Contents


Introduction  
0.1 Few-Shot Learning  
0.1.1 The Genesis  
0.1.2 Utility and Role in Artificial Intelligence  
0.2 Convolutional Neural Networks  
0.2.1 History and Architectures of Convolutional Neural Networks  
0.3 Introduction to the Experimental Part and the Generation-0 Algorithm of [1]  
0.3.1 Description of the Generation-0 Algorithm  
0.3.2 Related Research - Similar Works in International Literature  
0.4 Structure of the Thesis  

I. Theoretical Part  
Chapter 1 Convolutional Neural Networks  
1.1 Types of Learning  
1.1.1 Supervised Learning  
1.1.2 Unsupervised Learning  
1.1.3 Reinforcement Learning  
1.1.4 Self-supervised Learning  
1.2 Structure and Function of Convolutional Networks  
1.2.1 Structure and Layers of Convolutional Neural Networks  
1.2.2 Convolution Layer and Its Function  
1.2.3 Volumetric - Depth Convolution Processing  
1.2.4 Pooling Layer Function  
1.2.5 Batch Normalization Function  
1.2.6 Dropout Layer Function  
1.2.7 Useful Conclusions: Properties and Advantages  
1.3 Autoencoders  
1.3.1 Structure and Function  
1.3.2 Types of Autoencoders  

Chapter 2 Few-Shot Learning  
2.1 The Concept of Few-Shot Learning  
2.1.1 Technical Definition & General Approach to Few-Shot Learning  
2.1.2 Types of Processes  
2.1.3 Related Forms of Learning  
2.1.4 Common Datasets  
2.1.5 Mathematical Modeling of the Central Challenge of Few-Shot Learning  
2.2 Categorization of Few-Shot Learning Problems  
2.2.1 Focus on Data  
2.2.2 Focus on Model  
2.2.3 Focus on Algorithm  
2.3 Applications  
2.3.1 Computer Vision  
2.3.2 Robotics  
2.3.3 Natural Language Processing  
2.3.4 Acoustic Signal Processing  
2.3.5 Other Applications  

II. Experimental Part  
Chapter 3 Presentation of Experiments  
3.1 Structuring and Preparation  
3.1.1 Comparisons  
3.1.2 Few-Shot Categories  
3.1.3 Datasets  
3.1.4 Training – Experiment Details & Hyperparameters  
3.1.5 Evaluation on Few-Shot Task – Test Details & Hyperparameters  
3.2 Comparisons  
3.2.1 Comparison 1  
3.2.2 Comparison 2  
3.2.3 Comparison 3  
3.3 Conclusion and Future Work  
3.3.1 Assessment  
3.3.2 Future Endeavors

### Utilized Environment/Tools

- Python 3.x
- Jupyter Notebook
- Required libraries (listed in the `requirements.txt`)

### Utilized Datasets


## References


[1] Jathushan Rajasegaran et al., "Self-supervised Knowledge Distillation for Few-shot Learning", https://github.com/brjathu/SKD

[31] Resnets: He, Kaiming, et al. "Deep residual learning for image recognition." Proceedings of the IEEE conference on computer vision and pattern recognition. 2016.

[32] SE block: Hu, Jie, Li Shen, and Gang Sun. "Squeeze-and-excitation networks." Proceedings of the IEEE conference on computer vision and pattern recognition. 2018.

[63] Variational Autoencoder: Kingma, Diederik P., and Max Welling. "Auto-encoding variational bayes." arXiv preprint arXiv:1312.6114 (2013).


## Keywords

Data Science, Machine Learning (ML), Deep Learning(DL), Few-Shot Learning, Self-Supervised Learning, Computer Vision, Image Classification, Convolutional Neural Networks (CNNs), Artificial Neural Networks (ANNs), Autoencoders

