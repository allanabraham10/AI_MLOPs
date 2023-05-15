# Learning Objectives
At the end of the experiment you will be able to :
- understand what is object detection
- configure a state-of-the-art algorithm called YOLO V3
- make inferences from YOLO on real-time images

# Introduction

## What is YOLO V3?
YOLOv3 (You Only Look Once, Version 3) is a real-time object detection algorithm that identifies specific objects in videos, live feeds or images. The YOLO machine learning algorithm uses features learned by a deep convolutional neural network to detect an object. YOLO has the advantage of being much faster than other networks and still maintains accuracy.
The approach involves a single deep convolutional neural network (originally a version of GoogLeNet, later updated and called DarkNet based on VGG) that splits the input into a grid of cells and each cell directly predicts a bounding box and object classification. The result is a large number of candidate bounding boxes that are consolidated into a final prediction by a post-processing step.
It allows the model to look at the whole image at test time, so its predictions are informed by the global context in the image. Using CNN, YOLO can predict all objects in one forward pass and that is the reason for its full name “You Only Look Once”. You Only Look Once means it looks for the image/frame only once and is able to detect all the objects in the image/frame.
High-scoring regions are noted as positive detections of whatever class they most closely identify with. For example, in a live feed of traffic, YOLO can be used to detect different kinds of vehicles depending on which regions of the video score highly in comparison to predefined classes of vehicles.

## How YOLOv3 works?
The YOLOv3 network divides an input image into an S x S grid of cells and predicts bounding boxes as well as class probabilities for each grid. Each grid cell is responsible for predicting B-bounding boxes and C-class probabilities of objects whose centers fall inside the grid cell. Bounding boxes are the regions of interest (ROI) of the candidate objects. The “B” is associated with the number of using anchors. Each bounding box has (5 + C) attributes. The value of “5” is related to 5 bounding box attributes, which are center coordinates (bx, by) and shape (bh, bw) of the bounding box, and one confidence score. The “C” is the number of classes. The confidence score reflects how confident a box contains an object. The confidence score is in the range of 0 – 1.
Since we have an S x S grid of cells, after running a single forward pass convolutional neural network to the whole image, YOLOv3 produces a 3-D tensor with the shape of [S, S, B * (5 + C].
The following figure illustrates the basic principle of YOLOv3 where the input image is divided into the 13 x 13 grid of cells (13 x 13 grid of cells is used for the first scale, whereas YOLOv3 actually uses 3 different scales and we're going to discuss it in the section prediction across scale).

![image](https://github.com/allanabraham10/AI_MLOps/assets/69242466/a8925f49-26f1-4979-b0bf-220256f6bda1)

YOLOv3 was trained on the COCO dataset with C=80(class) and B=3(). So, for the first prediction scale, after a single forward pass of CNN, the YOLOv3 outputs a tensor with the shape of [(13, 13, 3 * (5 + 80)].
