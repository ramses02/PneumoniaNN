# PneumoniaNN

## Overview
This GitHub repository contains the code and documentation for a Pneumonia Detection project using deep learning techniques on X-ray images. The project aims to create a model capable of accurately detecting pneumonia from X-ray images and provides a comparative analysis of different model architectures. The repository includes code for data preprocessing, model building, and evaluation, as well as a detailed README to guide users through the project.

## Business Understanding

Pneumonia is a life-threatening respiratory condition that requires early and accurate diagnosis for effective treatment. Traditional diagnosis relies on manual interpretation of X-ray images by radiologists, which can be time-consuming and subject to human error. Automating this process using machine learning models can significantly improve diagnosis speed and accuracy, ultimately saving lives.

## Data Understanding

The dataset used in this project consists of 5233 X-ray images categorized into two classes: "Normal" and "Pneumonia." There is a significant class imbalance, with a larger number of images in the "Pneumonia" class. The goal is to build a model that can accurately classify X-ray images into these two classes.

## Models

After conducting an extensive evaluation of various models, including a baseline model, dense neural network, and convolutional neural network (CNN), employing diverse strategies such as regularization, layer dropout, and early stopping, we have carefully selected a subset of models for closer examination based on our primary metric of interest, recall. Recall is of paramount importance in our context as it directly influences the accuracy of disease prediction.

Upon thorough analysis of the performance metrics displayed in the visualization above, it becomes evident that our CNN model surpasses all others, achieving an exceptional accuracy and recall score of 100%. Consequently, our focus has shifted toward the CNN model as our primary candidate.


![metrics](https://github.com/ramses02/PneumoniaNN/blob/main/Project%3APresentation_images/allmodels_metrics.png)

Below, we present the confusion matrix for the CNN model on the testing dataset, accompanied by the loss function and the aforementioned accuracy and recall metrics.

CNN metrics:

![CNNmetrics](https://github.com/ramses02/PneumoniaNN/blob/main/Project%3APresentation_images/CNN_metrics.png)

CNN Confusion matrix:

![CNNconfmat](https://github.com/ramses02/PneumoniaNN/blob/main/Project%3APresentation_images/CNN_confmatrix.png)



## Usage

To use this repository, follow these steps:

Clone the repository to your local machine:

git clone https://github.com/your_username/pneumonia-detection.git

Explore the Jupyter notebooks in the "Notebooks" directory to understand the project flow and execute code step by step.

Use the provided scripts for specific tasks, such as data preprocessing or model training.

Experiment with different model architectures, hyperparameters, and data augmentation techniques to further improve the model's performance.



## Conclusion

Automated pneumonia detection from X-ray images has the potential to revolutionize the healthcare industry by providing faster and more accurate diagnoses. This project demonstrates the effectiveness of deep learning models, especially Convolutional Neural Networks (CNNs), in this context. By continuously optimizing and fine-tuning the model, we can enhance its performance and contribute to better healthcare outcomes.

We encourage contributions and feedback from the open-source community to further advance this project and its impact on the medical field.

## Repository Structure

```
.
|-- Data/
|-- Project:Presentation_images/
|-- .gitignore
|-- LICENSE
|-- Notebook.ipynb
|-- README.md
|-- paul_scratch.ipynb
|-- presentation.pdf
|-- ramsi_scratch.ipynb
```
