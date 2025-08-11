# Military Object Detection

This repository contains the code and notebooks for a military object detection project. The goal is to train a custom object detection model to identify various military assets in images. The project utilizes the TensorFlow Object Detection API and is designed to run in a Google Colab environment.

## Project Files
* model: contains checkpoint files of best trained model.

* Training_and_Detection.ipynb: This is the primary notebook used for training, evaluation, and testing the custom object detection model. It includes steps for setting up the environment, downloading the dataset, configuring the training pipeline, and visualizing the detection results.

* Loading_Model_and_Detection.ipynb: This notebook is a separate, simplified file for loading and testing a pre-trained model. It allows for quick inference on new images without needing to go through the entire training process.

* README.txt: A simple text file with notes on how to run the project.

## Getting Started
### Prerequisites
* Google Colab: The notebooks are specifically configured to run on Google Colab.

* Trained Model: To use Loading_Model_and_Detection.ipynb, you must have a trained model. The original Training_and_Detection.ipynb notebook is used to create this model.

### How to Run
* Clone this repository to your local machine or directly within your Google Colab session.

* Upload the coursework_model.zip file to your Colab content folder. The Loading_Model_and_Detection.ipynb notebook is designed to unzip and use this model.

* Open Loading_Model_and_Detection.ipynb in Colab and run the cells in order to test the detection on a sample image.

* To change the image, upload your image to the militaryImages/images/ folder and update the Image_Path variable.

## Model and Dataset
* Model: The project uses a ssd_mobilenet_v2_fpnlite_640x640 pretrained model from the TensorFlow Model Zoo as a base. A custom model named my_ssdmobnet2_IOU0.5 is trained on top of this.

* Dataset: The dataset used for training the model is hosted on Roboflow. You can find the dataset at the following URL: https://universe.roboflow.com/uni-awhxd/military-dataset-vormc
