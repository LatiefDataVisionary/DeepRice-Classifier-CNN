# DeepRice-Classifier-CNN

This repository contains a comprehensive deep learning project focused on the automated classification of rice varieties. The project utilizes a custom Convolutional Neural Network (CNN) architecture to distinguish between five distinct rice types with high precision. The system is designed to provide an efficient and scalable solution for agricultural quality control and industrial food processing.

## Project Overview

The primary objective of this project is to develop an automated vision system capable of identifying rice varieties based on their morphological features. By leveraging deep learning, this system reduces the dependency on manual inspection, which is often prone to human error and inefficiency. The model is trained on the Rice Image Dataset, which includes 75,000 high quality images of five rice varieties: Arborio, Basmati, Ipsala, Jasmine, and Karacadag.

## Key Features

*   **Custom CNN Architecture**: A lightweight and efficient sequential model designed specifically for single object classification against uniform backgrounds.
*   **Data Engineering Pipeline**: Implements stratified subsampling and high performance data loading using TensorFlow to ensure optimal hardware utilization.
*   **Robust Preprocessing**: Includes dynamic image augmentation and pixel normalization to enhance model generalization.
*   **Deployment Ready**: The project includes export pipelines for SavedModel, TensorFlow Lite, and TensorFlow.js, enabling deployment on servers, mobile devices, and web browsers.

## Dataset Information

The model is trained on the Rice Image Dataset by Murat Koklu et al. The dataset is perfectly balanced with 15,000 images per class, ensuring that the model does not develop bias toward any specific variety.

### Figure 1: Confusion Matrix
![Confusion_Matrix.png](https://github.com/LatiefDataVisionary/DeepRice-Classifier-CNN/blob/main/assets/Confusion%20Matrix%20-%20Klasifikasi%20Varietas%20Beras.png)
*Caption: Figure 1. Confusion Matrix showing the model performance on the test set.*

## Model Performance

The custom CNN architecture achieved an outstanding classification performance on the test set.

| Metric | Score |
| :--- | :--- |
| Test Accuracy | 99.13% |
| Precision | 0.9915 |
| Recall | 0.9913 |
| F1-Score | 0.9913 |

### Figure 2: Learning Curves
![learning_curves.png](https://github.com/LatiefDataVisionary/DeepRice-Classifier-CNN/blob/main/assets/learning_curves_DeepRice-Classifier-CNN.png)
*Caption: Figure 2. Training and Validation accuracy and loss curves.*

## Deployment Formats

This project provides multiple deployment artifacts to support various integration scenarios:

1.  **SavedModel**: Standard format for server side deployment and production inference.
2.  **TensorFlow Lite**: Optimized for edge devices and mobile applications.
3.  **TensorFlow.js**: Ready for client side integration in web applications.

## How to Run the Project

1.  Clone this repository to your local machine or Kaggle environment.
2.  Install the required dependencies using the provided requirements file:
    `pip install -r requirements.txt`
3.  Open the notebook located in the `notebooks/` directory.
4.  Ensure the dataset path in the configuration section points to your local dataset folder.
5.  Execute the cells sequentially to train the model and generate deployment artifacts.

## License

This project is licensed under the MIT License. See the LICENSE file for more information.

## Acknowledgments

Special thanks to Murat Koklu et al. for providing the Rice Image Dataset, which made this research possible.
