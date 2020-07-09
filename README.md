# Project Overview

In this project, we will attemp to build a pipeline that can be used within a web or mobile app to process real-world, user-supplied images. 

The main goal is to construct an image classifier that can differentiate dog's breeds. The model will:
* Accept input from either dog or human image;
* Output predictions of dog's breed if the image is detected to be a dog;
* Output predictions of most resembling dog's breed if the image is detected to be a human.

# File Distribution

## dog_app.ipynb

The `dog_app.ipynb` and `dog_app.html` are the original files for development. Although constructing models in Jupyter Notebook is extremely troublesome especially for large-scale data, we choose it because it's better for presentation purpose. You can find detailed instructions and explanations in the `dog_app.ipynb` about each step of constructing the pipeline.

## model_artifacts

The `model_artifacts` folder contains the weights for the trained CNN models used for this project. Because the training process will probably take viewers a considerable amount of time, feel free to use this and test the model without training the model. Specifically, for `STEP 3` and `STEP 4`, comment out the `train()` code block, and only run the `model.load_dict()` code block.

## Capstone_Report

The `Capstone Report` file contains an integrated compilation of all the work done for this project. It demonstrates the project in different steps of constructions, and also provide introductions to the background of the models used in this project. I recommend reading this report if you are really interested in the thought process of developing this project.

## Dataset for Training

The original dataset used for training is stored in Amazon S3 buckets. Please download through [the dog's dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip); [the human's dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip)

# Sample Output:



# Tech stack:

* PyTorch
* Numpy
* Pandas
* Matplotlib
* cv2, OpenCV's implementation of [Haar feature-based cascade classifiers](https://docs.opencv.org/trunk/d7/d8b/tutorial_py_face_detection.html)
* [VGG-16](https://neurohive.io/en/popular-networks/vgg16/)
* [ResNet50](https://www.mathworks.com/help/deeplearning/ref/resnet50.html)


