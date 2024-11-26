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


# Results:
Best Activation Function: tanh consistently provided better and more stable results compared to ReLU and Softplus. The enhanced images retained natural colors and balance.

Loss Visualization: The graph shows a steady decrease in training and validation loss, indicating good performance.

This project showcases the ability of deep learning to enhance images, with activation functions playing a key role in the quality of results.

(Model 1 : ReLU, Model 2 : Tanh, Model 3 : Softplus)

# Test 1:
![image](https://github.com/user-attachments/assets/dea4cd19-f853-4bdb-b2d9-3d7555ffaa12),![image](https://github.com/user-attachments/assets/2f33627c-cd85-4cfa-929b-5a0bc6180cd2),![image](https://github.com/user-attachments/assets/45c026de-8739-44cb-982f-34a87ab8d659),![image](https://github.com/user-attachments/assets/461c7dc0-15aa-42f6-9b12-b2844af30bb7)

# Test 2:
![image](https://github.com/user-attachments/assets/a24db8be-5ec9-48a2-91c5-fba112722d0b),![image](https://github.com/user-attachments/assets/d0e8a60b-b21f-48e1-a2c5-6957164d7c73),![image](https://github.com/user-attachments/assets/d8affd9d-42e9-4b20-bf1b-2d51a7d31b25),![image](https://github.com/user-attachments/assets/7964f7b4-1986-4348-8c10-c34768766a0f)

# Test 3:
![image](https://github.com/user-attachments/assets/cb17655f-9def-4dfe-8fd2-5b4deb7c89c4),![image](https://github.com/user-attachments/assets/946255bb-f9a7-4a80-a503-462456867a4a),![image](https://github.com/user-attachments/assets/90bd9663-95e9-440d-a774-86596db4d771),![image](https://github.com/user-attachments/assets/1b462690-94ee-4bab-8127-556bb7bbe9be)



# Conclusion:
Using softplus changes the way pixel values are processed because it amplifies them in a non-linear way. This can distort how the Red, Green, and Blue (RGB) channels combine, making the colors look different.

Think of it like turning up certain colors too much while dimming others, so the final image's color balance is off. To fix this, it's better to use relu, which is simpler and keeps the colors more natural.

ReLU works like a filter that only lets positive numbers through and blocks all negative numbers by turning them into zero.

Imagine shining a flashlight on a surface—only the parts in the light are visible (positive values), and everything in the dark is ignored (negative values). This keeps things simple and avoids adding extra complexity, making it great for image-related tasks because it doesn’t mess up the colors or features much.


Tanh (Hyperbolic Tangent) works like a squishing function that takes any input and maps it to a value between -1 and 1.

Think of it like stretching a rubber band so that extreme negative values are pulled closer to -1 and extreme positive values closer to 1, while values near zero stay around zero. This makes it useful for balancing data, especially when you want both negative and positive signals to matter.


# Comparison :
ReLU is best for speed and simplicity, tanh excels in balance and consistency, while softplus is smoother but may distort outputs like image colors.




# Training Data Set Link : 
https://www.kaggle.com/datasets/adityachandrasekhar/image-super-resolution
