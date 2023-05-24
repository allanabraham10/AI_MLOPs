## Learning Objectives:
At the end of the experiment, you will be able to:
- understand, prepare, and visualize the the dataset containing image and corresponding masked image used for segmentation
- implement DeepLabV3+ architecture
- create a masked image (prediction)

## Introduction
Semantic segmentation is a computer vision task that involves dividing an image into different regions, each of which is labeled with a semantic category. The goal of semantic segmentation is to enable machines to understand the content of an image at a pixel level, by assigning a label to each individual pixel based on the object or region it belongs to.
This technique is widely used in many applications such as self-driving cars, medical image analysis, and object recognition in robotics. It helps to extract meaningful information from images and to understand the relationships between objects and their environment.
The below figure shows how semantic segmentation differs from other algorithms, such as object detection.

![image](https://github.com/allanabraham10/AI_MLOps/assets/69242466/f5e9b4d7-82f3-46e5-8ef8-7a906b5380d1)

Moreover, in contrast to object detection, which detects and localizes objects within an image, semantic segmentation is more precise and detailed. It provides a much more granular understanding of the content of an image, allowing for more advanced and accurate applications.

## Dataset
The dataset is made up of images and segmentated mask from two diffrent sources- Shenzhen and Montgomery dataset
The CXR_png folder consists of Chest X-Rays and the masks folder has the segmented mask
There are 704 images with their masks mapped with each other

## Problem Statement
Perfrom the lungs segmentation on Chest X-Ray dataset using DeepLabV3+ model.
