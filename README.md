# Project 2 - Neural Networks for Object Detection by Almog and Rani

## Overview

This project demonstrates the implementation and application of a neural network for object detection, specifically focusing on detecting trains and airplanes within images. Utilizing the PASCAL VOC 2012 dataset and a ResNet18 backbone architecture, we present our methodology, experiments, and results in both image classification and object bounding box prediction.

## Project Structure

- **Backbone Selection:** we chose ResNet18 as our backbone architecture. 
  
- **Dataset:** We used the PASCAL VOC 2012 dataset, preprocessing it to focus on two classes: trains and airplanes. The dataset is renowned for its diverse range of images and annotations, providing a robust foundation for our object detection model.

- **Architecture:** Our model architecture is dual-headed, with one head for classification (determining if an image contains a train or an airplane) and another for bounding box detection (locating the object within the image).

- **Loss Functions and Metrics:** We employed Cross Entropy loss for classification and SmoothL1Loss for bounding box detection, alongside accuracy and intersection-over-union (IoU) metrics for performance evaluation.

- **Data Augmentation:** Techniques such as random greyscaling, Gaussian blur, color jitter, resizing, and normalization were applied to enhance model robustness.

- **Training:** Our model training utilized the SGD optimizer with momentum and L2 regularization. We carefully selected the learning rate and batch size to balance convergence speed and model stability.

- **Results:** Post-training, our model achieved a classification accuracy of 93% and a bounding box detection accuracy of 77% (based on IoU calculations). These results underscore the model's effectiveness and the successful application of our training methodology.

## Key Findings

- The pre-trained ResNet18 model, even when fine-tuned, demonstrated limitations in classification accuracy due to dataset specificity. However, with targeted training and architectural adjustments, significant improvements in performance were observed.
  
- Data augmentation and the choice of loss functions played critical roles in enhancing model generalization and reducing overfitting.

- Our model showcased high accuracy in both classification and object detection tasks, evidencing the efficacy of our chosen architecture and training strategy.

## Usage

### Video Demonstration

A video demonstration of our model's performance can be found at the following link, showcasing real-time object detection:




[Video Result](https://drive.google.com/file/d/1-32krIqy26KvwPDVVx6UEqiP4a-FHrQU/view?usp=sharing)

This video provides a visual representation of the model's capability to accurately identify and locate trains and airplanes in a dynamic context.

### How to Run

To replicate our experiments or utilize the model for similar object detection tasks, follow the detailed setup and execution instructions provided in our project repository. Ensure that the PASCAL VOC 2012 dataset is correctly setup and that the necessary Python packages for PyTorch and other dependencies are installed.

## Conclusion

This project illustrates the potential of neural networks in the field of object detection. Through meticulous architecture selection, dataset preparation, and model training, we demonstrated that even relatively simple models like ResNet18 can achieve high levels of accuracy in specific object detection tasks. Our findings contribute to the broader understanding of neural network applications in image classification and object detection, offering insights into model training and optimization strategies.

