# Image-Classification-using-Keras

# Overview
To build an image recognition model which is capable of identifying the pattern on a dress image.

# Dataset Information : 
❏ This dataset contains links to images of women's dresses.

❏ The corresponding images are categorized into 17 different pattern types.

❏ Most pattern categories have hundreds to thousands of examples.


# Tools And Technologies
1) Anaconda — Anaconda is a free and open source distribution of the Python and R programming languages for data science and machine  learning related applications, that aims to simplify package management and deployment. You can download it from the link below according to your system https://www.anaconda.com/download/

2) Tensorflow — TensorFlow is an open-source software library for dataflow programming across a range of tasks. Download link — https://www.tensorflow.org/install/install_windows

3) Keras — Keras is an open source neural network library written in Python. Activate Tensorflow env and install keras using:
pip install keras

4) CNN — Convolution Neural network , a class of deep, feed-forward artificial neural networks, most commonly applied to analyzing visual imagery.

# Steps

* You can find the problem statement and csv file with image links and labels at https://assignments.greendeck.co/assignments/

* I downloaded the images from the URL in the .csv file using the Python library called "urllib.request" and saved them into their respective label directories.

* Divided the images to Train, Validation and Test directories.

* Built a CNN model Architecture with 5 convolutional layers, 5 pooling layers and 3 dense layers.

* After training it I got the following accuracies:
    * Training Data - 68.96%
    * Validation Data - 69.74%
    * Test Data - 68.09%

* This the best accuracy I was able to get after applying different cnn models and even after using transfer learning. The dataset contained 15702 images with imblanced classes. I tried giving class weights but that brought my accuracy down to 10-20%. I still believe we can improve the accuracy of this model, any suggestion will be appreciated.

# Files in this Repository

* dress_patterns.csv - CSV file containing links of Images
* Loading_Images_From_the_Link.ipynb - Downloading images from the URL
* Dress_Pattern_Recognition_And_Classification.ipynb - Contains the preprocessing and Cnn Model
* Dress Similarity.ipynb - Testing the model with unknown images and showing similar dress pattern images
* cnn_model_architecture.json - Model architecture
* cnn_model_weights.h5 - Model weights
* Accuracy Plots.png - Training Accuracy vs Validation Accuracy
* Loss Plots.png - Training Loss vs Validation Loss

Please find the model jupyter notebook with interactive plots [here](https://nbviewer.jupyter.org/github/Shaan224/Dress-Pattern-Recognition-and-Image-Classification-using-Keras/blob/master/Dress_Pattern_Recognition_And_Classification.ipynb)
