# Household Object Image Detection
## Goal 
The goal of this project was to determine how can we utilize a model to identify
the main subject/object of an image. Our motivation for using object identification is from using facial and activity recognition, and providing the opportunity to help those with visual impairments by identifying videos and images on behalf of them.

This project contains data from CalTech dataset utilizing objects to train/test Computer Vision models. The dataset included ~500 total JPG images divided into “Train” and “Test” folders. For purposes of analysis, we only utilized the “Test” folder. Our data cleaning procedure consisted of going through image files and ensured all images were clear with at least 1 distinguishable subject. As you can see in our data dictionary below, our column consisted of the image name, the description was the image of a household object, and the potential response is a JPG image file.
 
## SRC 
### Installing/Building Code
To build this code, we imported numpy and tensorflow, specifically mobilenet_v2 in tensorflow. We created a function where we process the image and then use tensorflow's pretrained model to detect objects in the images from our dataset. 

### Usage 
We passed in each image into the model and the model would output the top three objects detected along with its confidence level for each prediction. We used the object identification code in Tensorflow to apply a pre-trained model that we found online, to our dataset. Mobilenettv2 within Tensorflow is a pre-trained network that is able to classify images into 1000 predetermined categories. With our dataset, for example, an JPG image of a toilet was presented to the model, and the model’s output would give us a couple of ideas of what it could be. It would say, for example, toilet, trash can, and bucket in a row. 

## Data Dictionary
| Column| Description| Potential Reponses|                   
|-------|------------|-------------------|
|Image Name | Image of household object.|JPG Image file.|

## Figures
| Figure Name| Description| Summary|                   
|-------|------------|-------------------|
|Figure1 | descibe it |summarize takeaways.|

## References 
Mobilenetv2: https://www.tensorflow.org/api_docs/python/tf/keras/applications/mobilenet_v2/MobileNetV2

Tensorflow: https://www.tensorflow.org/hub/tutorials/object_detection

Project 2 MI 1: https://docs.google.com/document/d/1OU50i-dGndjSv4O_4DIlQVNv_KLcjodPBuStC2pfFhI/edit?usp=sharing

Project 2 MI 2: https://docs.google.com/document/d/1DZCUWmKi0qrNylDYpL4U6qFQCZXf15twuvQ8tF2yLPY/edit?usp=sharing
