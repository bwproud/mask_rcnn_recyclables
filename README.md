# Detection of Recyclable Objects using MaskRCNN

Our goal was to develop a model that can detect and classify classes of recyclable items. The classes of recyclables that we currently support are plastic bottles, glass bottles, and metal soda cans. We trained a Mask RCNN model with a Resnet 101 backbone to serve as an object detection system that detects, bounds, and segments these classes.

## Getting Started

Unfortunately, due to how complex it is to train a Mask RCNN model, it's not much help to have this running locally. To truly test out our model, open the Mask_RCNN_Colab_Notebook.ipynb file in Google Colab, an online python interpreter (like Jupyter) that allows you to run code on a 12 core gpu.

## Files
### ML_Final_Project.pdf
### Mask_RCNN_Colab_Notebook.ipynb
### examples
### data.zip
### mrcnn
### detect_recyclables.py

## Authors

* **Brennan Proudfoot** 
* **Jay Rao** 

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Matterport for their Mask RCNN implementation
* VGG for their segmentation tool