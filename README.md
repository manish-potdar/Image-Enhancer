# Image Enhancer Project
This project is an image resolution enhancer built using a deep neural network. The network processes low-resolution images and produces enhanced high-resolution versions.

# Features
Deep Network Layers: The model consists of convolutional, up-sampling, and pooling layers to extract features and reconstruct the image.

# Three Activation Functions Tested:
ReLU: Efficient and fast but loses negative signals, which can affect balance.

Softplus: Smooth but tends to distort outputs, such as image colors.

Tanh: Balanced and consistent, providing the most reliable results in this project.

# Model Architecture:

![WhatsApp Image 2024-11-26 at 11 42 13 PM](https://github.com/user-attachments/assets/6d5751d0-e061-44a3-a875-6bd66912d08e)


Results
Best Activation Function: tanh consistently provided better and more stable results compared to ReLU and Softplus. The enhanced images retained natural colors and balance.
Loss Visualization: The graph shows a steady decrease in training and validation loss, indicating good performance.
This project showcases the ability of deep learning to enhance images, with activation functions playing a key role in the quality of results.

# Training Data Set Link : https://www.kaggle.com/datasets/adityachandrasekhar/image-super-resolution
