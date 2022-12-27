# Image_Segmentation

![image](https://user-images.githubusercontent.com/101316217/209589527-dc432ac2-3fe9-4547-95a4-0bdd4e47fdda.png)


## What Is Image Segmentation?
Image segmentation is a method of dividing a digital image into subgroups called image segments, reducing the complexity of the image and enabling further processing or analysis of each image segment. Technically, segmentation is the assignment of labels to pixels to identify objects, people, or other important elements in the image. 

A common use of image segmentation is in object detection. Instead of processing the entire image, a common practice is to first use an image segmentation algorithm to find objects of interest in the image. Then, the object detector can operate on a bounding box already defined by the segmentation algorithm. This prevents the detector from processing the entire image, improving accuracy and reducing inference time.

Image segmentation is a key building block of computer vision technologies and algorithms. It is used for many practical applications including medical image analysis, computer vision for autonomous vehicles, face recognition and detection, video surveillance, and satellite image analysis.

## What is UNET?
UNET is an architecture developed by Olaf Ronneberger et al. for Biomedical Image Segmentation in 2015 at the University of Freiburg, Germany. It is one of the most popularly used approaches in any semantic segmentation task today. It is a fully convolutional neural network that is designed to learn from fewer training samples. It is an improvement over the existing FCN — “Fully convolutional networks for semantic segmentation” developed by Jonathan Long et al. in (2014). 

![image](https://user-images.githubusercontent.com/101316217/209589247-9d2fbf0f-1247-4fc0-a6c8-53ae1937f4e2.png)


## Training  

the main parameters:

ENDCODER = 'timm-efficientnet-b0'   # encoder of the efficientnet


WEIGHTS = 'imagenet'                # weights of imagenet

num_epochs = 25

## Results 

train_loss : 0.09031671633323034 valid_loss : 0.16858898475766182


![image](https://user-images.githubusercontent.com/101316217/209589509-6e41232b-c5fe-421b-b2cf-d941de506536.png)


## Datasets sources 

http://www.kalmasoft.com/KMAPS/molindx.htm

## Future Work

implementing Unet from scratch 
using different types of encoders 
