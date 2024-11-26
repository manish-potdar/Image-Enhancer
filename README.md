# Image Enhancer Project
This project is an image resolution enhancer built using a deep neural network. The network processes low-resolution images and produces enhanced high-resolution versions.

# Features
Deep Network Layers: The model consists of convolutional, up-sampling, and pooling layers to extract features and reconstruct the image.

# Three Activation Functions Tested:
ReLU: Efficient and fast but loses negative signals, which can affect balance.
Softplus: Smooth but tends to distort outputs, such as image colors.
Tanh: Balanced and consistent, providing the most reliable results in this project.

Training & Validation Graph: Included for visualizing the range of training and validation loss over epochs.
Model Architecture
Layer (Type)	Output Shape	Param #
Conv2D (64 filters)	(None, 128, 128, 64)	1,792
UpSampling2D	(None, 256, 256, 64)	0
Conv2D (128 filters)	(None, 256, 256, 128)	73,856
MaxPooling2D	(None, 128, 128, 128)	0
Conv2D (64 filters)	(None, 128, 128, 64)	73,792
UpSampling2D	(None, 256, 256, 64)	0
Conv2D (128 filters)	(None, 256, 256, 128)	73,856
MaxPooling2D	(None, 128, 128, 128)	0
Conv2D (64 filters)	(None, 128, 128, 64)	73,792
Conv2D (Output, 3 filters)	(None, 128, 128, 3)	1,731
Results
Best Activation Function: tanh consistently provided better and more stable results compared to ReLU and Softplus. The enhanced images retained natural colors and balance.
Loss Visualization: The graph shows a steady decrease in training and validation loss, indicating good performance.
This project showcases the ability of deep learning to enhance images, with activation functions playing a key role in the quality of results.

# Training Data Set Link : https://www.kaggle.com/datasets/adityachandrasekhar/image-super-resolution
