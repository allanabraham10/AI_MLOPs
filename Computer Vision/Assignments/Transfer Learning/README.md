# Learning Objectives:
At the end of the experiment, you will be able to:
- Understand and use a pre-trained model
- Fine-tune the top layers while using a pre-trained model

# Introduction
A common and highly effective approach to deep learning on small image datasets is to use a pre-trained model.

If the original dataset is large enough and general enough, the spatial hierarchy of features learned by the pre-trained model can effectively act as a generic model of the visual world, and hence, its features can prove useful for many different computer vision problems even though these new problems may involve completely different classes than those of the original task.

There are two ways to use a pre-trained model:
- feature extraction and
- fine-tuning

# Feature extraction
A CNN typically consists of a:
- Convolutional base
- Densely connected classifier

# Key Idea -
- Features are learned by the convolutional base. So reuse it.
- Train a new classifier for your problem

![image](https://github.com/allanabraham10/AI_MLOps/assets/69242466/9b521563-51e7-41fd-b945-9afafd75b9f2)
