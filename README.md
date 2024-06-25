---

# Prodigy-ML-04

**Crafted With Love by Sam Naveenkumar .V**

[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Overview

Welcome to **Prodigy-ML-04**, a comprehensive hand gesture recognition model designed to accurately identify and classify different hand gestures from image or video data. This project aims to enable intuitive human-computer interaction and gesture-based control systems, making technology more accessible and interactive.

## Features

- **Accurate Gesture Recognition**: Leverage a convolutional neural network (CNN) to classify hand gestures with high accuracy.
- **Real-time Predictions**: Integrate with webcam or video feed to provide real-time gesture recognition.
- **Easy to Use**: Simple and clean code structure for easy understanding and modification.
- **Extensible**: Easily extend the model to include more gestures or improve accuracy with additional data.

## Dataset

This project uses the Leap Gesture Database from Kaggle, which can be found [here](https://www.kaggle.com/datasets/gti-upm/leapgestrecog).

## Getting Started

### Prerequisites

- A Google account to use Google Colab.
- Basic understanding of Python and machine learning concepts.

### Using the Colab Notebook

1. **Open the Colab Notebook**:

2. **Setup Kaggle API Key**:

   To download the dataset, you'll need a Kaggle API key. Follow these steps:

   - Sign in to your Kaggle account.
   - Go to `Account` and select `Create New API Token` to download the `kaggle.json` file.
   - Upload the `kaggle.json` file in the Colab notebook.

3. **Run the Notebook**:

   Execute each cell in the notebook sequentially. The notebook includes:

   - **Downloading the Dataset**: Automatically download and unzip the dataset from Kaggle.
   - **Training the Model**: Train the hand gesture recognition model using the provided dataset.
   - **Real-time Predictions**: Use the webcam to make real-time gesture predictions or upload an image/video for prediction.

4. **Saving and Loading the Model**:

   The trained model will be saved to your Google Drive. You can load the saved model for future predictions without retraining.

## Model Architecture

The model uses a convolutional neural network (CNN) with the following architecture:

- **Conv2D**: 32 filters, 3x3 kernel, ReLU activation
- **MaxPooling2D**: 2x2 pool size
- **Conv2D**: 64 filters, 3x3 kernel, ReLU activation
- **MaxPooling2D**: 2x2 pool size
- **Conv2D**: 128 filters, 3x3 kernel, ReLU activation
- **MaxPooling2D**: 2x2 pool size
- **Flatten**
- **Dense**: 128 units, ReLU activation
- **Dropout**: 50%
- **Dense**: 8 units, Softmax activation (for 8 gesture classes)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an Issue to improve this project.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- The dataset used in this project is provided by [Leap Gesture Database](https://www.kaggle.com/datasets/gti-upm/leapgestrecog) on Kaggle.
- Special thanks to the contributors and the open-source community for their valuable resources and support.

---
