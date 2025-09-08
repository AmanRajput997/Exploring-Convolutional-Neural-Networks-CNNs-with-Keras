# Exploring-Convolutional-Neural-Networks-CNNs-with-Keras
A Convolutional Neural Network is a class of deep neural networks most commonly applied to analyzing visual imagery. They are inspired by the biological processes in the animal visual cortex. CNNs use special layers—convolutional and pooling layers—to automatically and adaptively learn spatial hierarchies of features from input images

This means they can learn to detect simple patterns like edges in the initial layers, which are then combined to form more complex patterns like shapes, and eventually, recognizable objects in deeper layers


✨  Core Concepts Demonstrated:
This repository breaks down the essential building blocks of a CNN architecture.

1. Padding [(Keras_Padding_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Keras_Padding_Demo.ipynb):In a convolutional layer, the filter (or kernel) slides over the input        image. Padding deals with how to handle the borders of the image.

  •  padding='valid': (Default) This means no padding is added. The filter is only applied to "valid" positions where it fully overlaps with the input. This causes the output feature map to be smaller than the input.

  •  padding='same': This adds padding (typically zeros) around the input image, so the output feature map has the same spatial dimensions as the input. This is useful for preserving the size of the feature maps through the network.

2. Strides [(Keras_Strides_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Keras_Strides_Demo.ipynb)

   •  strides=(1, 1): (Default) The filter moves one pixel at a time.

   •  strides=(2, 2): The filter moves two pixels at a time, both horizontally and vertically. A larger stride results in a smaller output feature map, effectively downsampling the image and reducing the number of computations.

3. Pooling [(Keras_Pooling_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/Keras_Pooling_Demo.ipynb):Pooling layers are another way to downsample the feature maps. Their goal is to reduce the spatial dimensions, which decreases the number of parameters and computations in the network. This also helps in making the detected features more robust to changes in their position in the image.

  •  Max Pooling [(MaxPooling2D)](https://keras.io/api/layers/pooling_layers/max_pooling2d/): Takes the maximum value from the pool (the area of the feature map covered by the filter). It's effective at capturing the most prominent features.

  •  Average Pooling [(AveragePooling2D)](https://keras.io/api/layers/pooling_layers/average_pooling2d/): Takes the average of all values in the pool. It provides a smoother downsampling.


🏛️ Architecture Demo: LeNet-5[(LeNET_Arch_Demo.ipynb)](https://github.com/AmanRajput997/Exploring-Convolutional-Neural-Networks-CNNs-with-Keras/blob/main/LeNET_Arch_Demo.ipynb)
The LeNet-5 architecture is one of the earliest and most foundational CNNs, developed by Yann LeCun in 1998 for handwritten digit recognition. This notebook demonstrates how to build this classic architecture, combining all the concepts above:

1. Convolutional Layer (tanh activation)

2. Average Pooling Layer

3. Convolutional Layer (tanh activation)

4. Average Pooling Layer

5. Flatten Layer (to convert 2D feature maps into a 1D vector)

6. Dense (Fully Connected) Layers for classification

This demo serves as a great example of how these individual components come together to form a complete and effective neural network.



  
