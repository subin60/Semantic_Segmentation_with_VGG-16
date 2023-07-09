Autonomous Vehicle Semantic Segmentation with VGG-16

This project demonstrates the implementation of semantic segmentation in autonomous vehicles using a VGG-16 backbone network and TensorFlow. Semantic segmentation refers to the process of partitioning an image into constituent parts or objects and classifying each part or pixel into a class label. This is particularly useful in the context of self-driving cars where we need to identify objects such as pedestrians, vehicles, trees, and roads.

Project Structure

The project follows the standard structure of a Machine Learning project:

- Import Libraries
- Load and preprocess the data
- Define the model
- Train the model
- Evaluate the model
- Generate segmentation masks for video frames

Model

The model used in this project is a Fully Convolutional Network (FCN) based on the VGG-16 architecture. VGG-16 was chosen due to its strong feature extraction capabilities and widespread use in the field. The FCN part of the model allows for end-to-end, pixel-to-pixel semantic segmentation, which provides a more detailed output than bounding box object detection methods.

Dataset

The dataset used for this project is the KITTI Vision Benchmark Suite, a comprehensive dataset for use in mobile robotics and autonomous driving. It includes a wide array of high-resolution sensor data for tasks such as stereo vision, optical flow, visual odometry, 3D object detection, and 3D tracking.

The dataset was recorded from a variety of sensor platforms, including high-resolution color and grayscale stereo cameras, a Velodyne 3D laser scanner, and a high-precision GPS/IMU inertial navigation system. For this project, we particularly use the data related to road and lane identification.


Results

The resulting model is capable of performing real-time semantic segmentation on video from a self-driving car perspective. The script also includes code for saving the output video with a transparent overlay of the predicted segmentation.

Dependencies

TensorFlow 2.x
OpenCV
Numpy
Matplotlib
Future Improvements

There are several areas for potential future improvements:

Training the model on a larger and more diverse dataset.
Tuning the model parameters to increase the accuracy.
Experimenting with other architectures like UNet, Mask R-CNN, or custom models.
Real-time implementation and testing on autonomous vehicles.

Acknowledgments

This project is inspired by the research paper "Fully Convolutional Networks for Semantic Segmentation" by Long, Shelhamer, and Darrell. The VGG16 model weights were obtained from the pre-trained models available in TensorFlow Keras.
