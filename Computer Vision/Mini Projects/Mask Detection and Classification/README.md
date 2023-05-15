# Learning Objectives
At the end of the experiment, you will be able to :
- load the image dataset using ImageDataGenerator from the path directory
- perform data augmentation on the fly and create batches of the dataset
- build the convolutional neural networks for classification problem
- visualize & interpret what CNN layers learn
- use the transfer learning (pre-trained models) for classification problems

# Introduction
This project uses a Deep Neural Network, more specifically a Convolutional Neural Network, to differentiate between images of people, with masks, without masks and incorrectly placed masks. Manually built and pretrained networks will be used to perform this classification task.

## Face-Mask-Detection-Using-CNN
- Outbreak of the Coronavirus pandemic has created various changes in the lifestyle of everyone around the world.
- Among these changes, wearing a mask has been very vital to every individual.
- Detection of people who are not wearing masks is a challenge due to the large populations.
- This face mask detection project can be used in schools, hospitals, banks, airports etc as a digitalized scanning tool.
  - The technique of detecting people’s faces and segregating them into three classes namely the people with masks and people without masks and partial masks is done with the help of image processing and deep learning.
- With the help of this project, a person who is monitoring the face mask status for a particular firm can be seated in a remote area and still monitor efficiently and give instructions accordingly.

![image](https://github.com/allanabraham10/AI_MLOps/assets/69242466/95544dfa-02de-4446-a202-738a3ad6b424)

# Dataset
The data for this mini-project is collected from various sources including the masked images from internet and general frontal face images considered as without mask. This dataset consists of 5029 train images and 1059 test images with 3 classes with_mask, without_mask and partial_mask
Many people are not correctly wearing their masks due to bad practices, bad behaviors or vulnerability of individuals (e.g., children, old people). For these reasons, several mask wearing campaigns intend to sensitize people about this problem and good practices. In this sense, this work proposes three types of masked face detection dataset
- Without Mask/ With Mask/ Partial Mask
Note that this dataset contains some annotated (artificially generated) masks to augment the 'masked' data category.

# Problem Statement
To build and implement a Convolutional Neural Network model to classify between masked/unmasked/partially masked faces.
