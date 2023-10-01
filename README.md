# Transfer Learning and Convolutional Neural Networks (TLCNN)

## Introduction
Image classification and the technologies it utilizes has boomed in popularity recently. A convolutional neural network (CNN) is a deep learning algorithm that excels at this task and has become the most popular model type for image classification.

This project explores some of the fundamental building blocks of CNNs and what makes them ideal for image classification. It does so with two example models built for two different datasets and discusses the results. Finally, some advantages and limitations of using transfer learning with CNNs are explored.

## Technologies
* Python 3.10.12
* Google Colab Pro with V100 GPU
* TensorFlow 2.12.0
* Keras 2.12.0

## Setup
To run the code in a reasonable amount of time requires access to hardware that can process neural networks with many parameters. I used Google's Colab Pro, but any applicable hardware (e.g., GPU or TPU) will do.

The two datasets are called CIFAR-10 and STL-10. Keras has CIFAR-10 available for direct download, but STL-10 needs to be download externally. Running [stl10_input.ipynb](https://github.com/DHoog4/CS767_Project/blob/master/stl10_input.ipynb) will download the images. If you are using Colab, the images need to be moved to Google Drive (since Colab is hosted on Google's cloud servers, it cannot access your machine's drive, but it can access your Google Drive). The second cell in 'CS767_Final_STL10_Hoogasian_Daniel.ipynb' mounts Google Drive to Colab. Line 37 in the third cell creates an object for the location of the images (my folder was titled 'img' and it was in the main 'MyDrive').

## Resources

* [STL-10 dataset](https://cs.stanford.edu/~acoates/stl10/)
* [CIFAR-10 dataset](http://www.cs.toronto.edu/~kriz/cifar.html)

## Room for Improvement

Room for improvement:
* Develop more customized, efficient CNN for CIFAR-10

To do:
* Implement transfer learning for both datasets, using a resizing layer