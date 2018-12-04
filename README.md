# Detection of Recyclable Objects using MaskRCNN

Our goal was to develop a model that can detect and classify classes of recyclable items. The classes of recyclables that we currently support are plastic bottles, glass bottles, and metal soda cans. We trained a Mask RCNN model with a Resnet 101 backbone to serve as an object detection system that detects, bounds, and segments these classes.

## Getting Started

Unfortunately, due to how complex it is to train a Mask RCNN model, it's not much help to have this running locally. To truly test out our model, open the Mask_RCNN_Colab_Notebook.ipynb file in Google Colab, an online python interpreter (like Jupyter) that allows you to run code on a 12 core gpu.

## Files/Folders
### [ML_Final_Project.pdf](ML_Final_Project.pdf)
This is our final project writeup which includes information on our task, our model, and our results.
### [Mask_RCNN_Colab_Notebook.ipynb](Mask_RCNN_Colab_Notebook.ipynb)
This is the Colab python notebook used to both train the model and test it on the validation/test set. Open this in Colab to try out the model for yourself.
NOTE: If you want to try out the model using our weights, you need to download our .h5 file from here: https://drive.google.com/file/d/1AunkAymLdhg-dgJYU4jddjcjF0XMxzzJ/view and then add it to your google drive where it will be accessed in the python notebook.
### examples/
This folder contains example inferences the model returned. Especially of note is demo.mp4 which is a video on which we ran our detection. 
### [data.zip](data.zip)
This zip contains the training, validation, and test data used in our project
### [mrcnn/](mrcnn)
This folder contains Matterport's Mask RCNN implementation. Only change we made here was to update the visualization code to keep mask colors consist across classes (to enable detection on videos) and to return the image with the bounding boxes and masking so it can be saved to a file locally.
### [detect_recyclables.py](detect_recyclables.py)
This file contains the custom training parameters and dataset extraction for our recycling task. Is customized to allow a user to adjust the number of epochs and the number of layers to train on
## Authors

* **Brennan Proudfoot** 
* **Jay Rao** 

## Acknowledgments

* Matterport for their Mask RCNN implementation
* VGG for their segmentation tool
