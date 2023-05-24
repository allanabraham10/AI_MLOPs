## Learning Objectives:
At the end of the experiment, you will be able to:
- understand, prepare, and visualize the the dataset containing image and corresponding masked image used for segmentation
- understand the encoder, bottleneck, and decoder region of a U-Net architecture
- build and train a U-Net architecture for segmentation
- create a masked image (prediction)
- calculate the accuracy score like IoU and Dice-Score used in segmentation
- understand and implement DeeplabV3+ architecture for segmentation

## Dataset
We will be training the model on the Oxford Pets - IIIT dataset. This contains pet images, their classes, segmentation masks, and head region of interest. We will only use the images and segmentation masks for this experiment.
The dataset consists of images of 37 pet breeds, with 200 images per breed (~100 each in the training and test splits). Each image includes the corresponding label and pixel-wise masks. The masks are class labels for each pixel. Each pixel is given one of three categories:
- Class 1: Pixel belonging to the pet.
- Class 2: Pixel bordering the pet.
- Class 3: None of the above/a surrounding pixel.
