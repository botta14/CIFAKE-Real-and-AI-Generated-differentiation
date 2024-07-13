# CIFAKE Project

The CIFAKE project is a comprehensive effort to develop and implement techniques for distinguishing between AI-generated images and real images. This project leverages a combination of preprocessing techniques, feature extraction, machine learning, and deep learning models to accurately classify images.

## Dataset

The dataset used for this project is available on Kaggle: [CIFAKE - Real and AI Generated Synthetic Images](https://www.kaggle.com/datasets/birdy654/cifake-real-and-ai-generated-synthetic-images).

## Project Phases

### 1. Data Exploration Phase

The data exploration phase involves:
- Loading the dataset.
- Analyzing its structure.
- Visualizing sample images.
- Computing various statistics to understand the dataset’s characteristics.

This phase helps identify any data quality issues and understand the distribution of the data.

### 2. Preprocessing Phase

The preprocessing phase involves:
- Resizing images.
- Applying Gaussian blurring.
- Sharpening images.
- Applying Contrast Limited Adaptive Histogram Equalization (CLAHE) to enhance image quality.

These techniques significantly improve the quality of images, making them more suitable for feature extraction and subsequent classification.

### 3. Feature Extraction Phase

The feature extraction phase is crucial for converting raw image data into a format suitable for machine learning algorithms. This phase involves:
- Using Scale-Invariant Feature Transform (SIFT) to extract key points and descriptors from the images.
- Creating feature histograms from these descriptors.

### 4. Machine Learning Phase

In this phase, the extracted features are used to train machine learning models. The steps include:
- Reducing dimensionality using Principal Component Analysis (PCA).
- Scaling the features.
- Applying various classifiers such as SVM, Logistic Regression, and an Ensemble Stacking Classifier.

### 5. Dimensionality Reduction

- PCA is used to reduce the feature dimensions while retaining 95% of the variance.

### 6. Deep Learning Phase

In this phase, two deep learning models were trained and evaluated:
- A custom Convolutional Neural Network (CNN).
- MobileNetV2, a pre-trained model.

Data augmentation was applied to improve generalization.

### 7. Results of Deep Learning Phase

The custom CNN and MobileNetV2 models were both trained and evaluated on the CIFAKE dataset. MobileNetV2 showed higher performance in terms of accuracy and AUC, demonstrating its effectiveness for this classification task. The ROC and Precision-Recall curves provided further insights into the models' performance.

## Installation and Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/botta14/CIFAKE-Real-and-AI-Generated-differentiation.git
    ```

2. Navigate to the project directory:
    ```bash
    cd CIFAKE-Real-and-AI-Generated-differentiation
    ```


3. Download the dataset from Kaggle and place it in the appropriate directory.

4. Run the project notebooks or scripts for each phase.

## Contributing

Contributions are welcome! Please contact me for more details on how to contribute to this project.

## Contact

For any questions or inquiries, please contact me at [botabatoot7@gmail.com](mailto:botabatoot7@gmail.com).

## Acknowledgments

- [Kaggle](https://www.kaggle.com) for providing the dataset.
