# Convolutional Neural Network for MNIST Digit Recognition Using RISC-V Vector ISA

## Project Overview
This project implements a Convolutional Neural Network (CNN) for recognizing handwritten digits from the MNIST dataset using RISC-V Vector ISA. The goal is to leverage the power of vectorized operations to achieve efficient processing and high accuracy in digit recognition.

## Architecture Details
The architecture of the CNN consists of several layers:
- **Input Layer**: 28x28 pixel grayscale images from the MNIST dataset.
- **Convolutional Layers**: Multiple layers where filters are applied to extract features from the input images.
- **Activation Layers**: Non-linear activation functions, typically ReLU (Rectified Linear Unit), applied after convolutional layers.
- **Pooling Layers**: Max pooling layers that reduce the spatial dimensions of the feature maps to retain essential information while reducing complexity.
- **Fully Connected Layers**: Layers that make the final prediction based on the features extracted by the convolutional layers.

## Methodology
1. **Data Preparation**: Load and preprocess the MNIST dataset, normalizing the pixel values.
2. **Model Construction**: Build the CNN architecture with appropriate layers for feature extraction and classification.
3. **Training**: Use backpropagation and an optimizer like Adam to train the model on the training dataset.
4. **Validation**: Monitor the model performance on a validation set to avoid overfitting.
5. **Testing**: Evaluate the trained model on the test dataset and record accuracy.

## Implementation Details
The implementation is optimized for RISC-V Vector ISA, allowing parallel processing of multiple data elements. Key components include:
- Efficient convolution operations using vectorization.
- Memory management strategies to optimize RAM usage during execution.
- Utilization of RISC-V specific instructions to enhance processing speed.

## Results
The model demonstrated an accuracy of over 98% on the MNIST test dataset. The efficiency of the algorithm on RISC-V architecture showcases the capability of handling deep learning tasks with minimal hardware resources.

## Setup Instructions
1. **Clone the Repository**: `git clone https://github.com/Alizawwaris974/CNN-for-Digit-Recognition.git`
2. **Navigate to Directory**: `cd CNN-for-Digit-Recognition`
3. **Install Dependencies**: Use the provided `requirements.txt` file to install necessary Python packages.
4. **Run the Model**: Execute the main script to start training and testing the model.

For any additional issues, please refer to the `docs` directory or reach out via the repository's Issues section.