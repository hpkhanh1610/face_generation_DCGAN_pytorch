# Face Generation using Deep Convolutional Generative Adverasial Network (DCGAN) in PyTorch

In this project, we'll define and train a DCGAN on a dataset of faces. The goal is to get a generator network to generate *new* images of faces that look as realistic as possible!

The project will be broken down into a series of tasks from **loading in data to defining and training adversarial networks**. At the end of the notebook, we'll be able to visualize the results of your trained Generator to see how it performs; our generated samples should look like fairly realistic faces with small amounts of noise.

### Get the Data

We'll be using the [CelebFaces Attributes Dataset (CelebA)](http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html) to train our adversarial networks.

This dataset is more complex than the number datasets (like MNIST or SVHN), and so, we should prepare to define deeper networks and train them for a longer time to get good results. It is suggested that we utilize a GPU for training.

### Pre-processed Data

Since the project's main focus is on building the GANs, the dataset has been pre-processed for us. Each of the CelebA images has been cropped to remove parts of the image that don't include a face, then resized down to 64x64x3 NumPy images. Some sample data is show below.

<img src='assets/processed_face_data.png' width=60% />

> If you are working locally, you can download this data [by clicking here](https://s3.amazonaws.com/video.udacity-data.com/topher/2018/November/5be7eb6f_processed-celeba-small/processed-celeba-small.zip)

This is a zip file that you'll need to extract in the home directory of this notebook for further loading and processing. After extracting the data, you should be left with a directory of data `processed_celeba_small/`
