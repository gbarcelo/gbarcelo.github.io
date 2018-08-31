---
layout: project
type: project
image: images/proj2_1.jpeg
title: UAS: Image Processing Using TensorFlow
permalink: projects/uas_tf
# All dates must be YYYY-MM-DD format!
date: 2018-05-13
labels:
  - Drone
  - Machine Learning
  - TensorFlow
  - Computer Vision
summary: An ongoing project aiming to draw useful information from images using computer vision and unmanned aerial vehicles.
---

Manual inspection of high-risk vegetation in remote areas to inspect high voltage electrical components is costly and dangerous. Our team's goal on this project is to substitute manual inspections either on-field or helicopter with drone co-processing.

This project is still in its early stages. In the semester of Spring '18, I performed research and experimentation on computer vision models with a team to find an accessible but powerful model. For the proof-of-concept, we chose to use the Faster R-CNN Resnet-50 pretrained model to retrain on a one-class dataset of “plant parts”. The dataset came from ImageNet and provided roughly 300 annotated images for training.
	The TensorFlow Object Detection API was developed by Google to enable experimentation using different parts of successful object detection/classification models with others. The Faster R-CNN is a method of bounding box prediction based on some extracted features, while Resnet is one state-of-the-art feature extractor made freely available. This combination was chosen for the proof-of-concept because of its average speed and average precision, versus other combinations of models with either slower speed and higher precision or faster speed and lower precision.
	Training must be done from scratch and takes many hours to get results. The model we trained was frozen after approximately 14,000 iterations, which took over 72 hours to train. Other iterations were tested before and after this checkpoint, but through trial and error this version was chosen for best performance. The results showed promise, however due to the differences between the training dataset and the test images, it was clear that we would need to build our own dataset from scratch to train a reliable model. We are currently in the process of this task as of Fall '18.

