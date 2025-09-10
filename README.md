# Exploring-Convolutional-Neural-Networks-CNNs-with-Keras
A Convolutional Neural Network is a class of deep neural networks most commonly applied to analyzing visual imagery. They are inspired by the biological processes in the animal visual cortex. CNNs use special layers—convolutional and pooling layers—to automatically and adaptively learn spatial hierarchies of features from input images.

This means they can learn to detect simple patterns like edges in the initial layers, which are then combined to form more complex patterns like shapes, and eventually, recognizable objects in deeper layers.


✨  Core Concepts Demonstrated: This repository breaks down the essential building blocks of a CNN architecture.

  1. Padding [(Keras_Padding_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Keras_Padding_Demo.ipynb): In a convolutional layer, the filter (or kernel) slides over the          input image. Padding deals with how to handle the borders of the image.

   •  padding='valid': (Default) This means no padding is added. The filter is only applied to "valid" positions where it fully overlaps with the input. This causes the output feature map to be smaller than the input.

   •  padding='same': This adds padding (typically zeros) around the input image, so the output feature map has the same spatial dimensions as the input. This is useful for preserving the size of the feature maps through the network.

  2. Strides [(Keras_Strides_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Keras_Strides_Demo.ipynb)

   •  strides=(1, 1): (Default) The filter moves one pixel at a time.

   •  strides=(2, 2): The filter moves two pixels at a time, both horizontally and vertically. A larger stride results in a smaller output feature map, effectively downsampling the image and reducing the number of computations.

  3. Pooling [(Keras_Pooling_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Keras_Pooling_Demo.ipynb):Pooling layers are another way to downsample the feature maps. Their       goal is to reduce the spatial dimensions, which decreases the number of parameters and computations in the network. This also helps in making the detected features more robust to changes in their position in the image.

   •  Max Pooling [(MaxPooling2D)](https://keras.io/api/layers/pooling_layers/max_pooling2d/): Takes the maximum value from the pool (the area of the feature map covered by the filter). It's effective at capturing the most prominent           features.

   •  Average Pooling [(AveragePooling2D)](https://keras.io/api/layers/pooling_layers/average_pooling2d/): Takes the average of all values in the pool. It provides a smoother downsampling.


🏛️    Architecture: 

   1. Classic Architecture: LeNet-5 [(LeNET_Arch_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/LeNET_Arch_Demo.ipynb):Explore the implementation of LeNet-5, one of the          earliest and most influential CNNs. This notebook is a perfect example of how the fundamental layers work together to create a complete image classification model

   2. Flexible Architectures: The Keras Functional API: The Functional API allows for the creation of more complex models, such as those with multiple inputs and outputs, or shared layers.

  • Introduction [(Functional_API_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Functional_API_Demo.ipynb):Get a basic introduction to the syntax and power of the             Functional API.

  • Handling Multiple Inputs [(Functional_API_Multiple_Input.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Functional_API_Multiple_Input.ipynb): Learn how to build models that     can process and integrate information from several different input sources simultaneously.

   3. Practical Example: Multi-Output Face Analysis [(Fuctional_Model_UTKFace.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Fuctional_Model_UTKFace.ipynb):
      This notebook provides a powerful, real-world example of the Functional API. It builds a multi-output model that predicts both the age and gender of a person from an image of their face, using the UTKFace dataset.

🚀 Part 3: Advanced CNN Techniques:Dive deeper into advanced methods for improving, debugging, and optimizing your models.

   1. Visualizing What CNNs Learn ([Visualizing_CNN.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Visualizing_CNN.ipynb):Ever wondered what's happening inside the "black box"        of a CNN? This notebook demonstrates how to:

  • Visualize Filters: See the actual patterns that each filter in your convolutional layers has learned to detect.

  • Visualize Feature Maps: Observe how the network activates in response to an input image, highlighting the features it finds important for its predictions.


   2. Transfer Learning with Pre-trained Models [(Pretrained_Models_(ResNet50)ipynb.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Pretrained_Models_(ResNet50)ipynb.ipynb):Why        train a model from scratch when you can stand on the shoulders of giants? Transfer learning is a powerful technique where you use a model pre-trained on a massive dataset (like ImageNet) and adapt it for your own task. This              notebook shows you how to:

  • Load and use a state-of-the-art pre-trained model (ResNet50).

  • Perform image classification on new images with just a few lines of code.










  
