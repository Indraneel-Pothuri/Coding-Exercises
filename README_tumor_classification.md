This notebook implements a comprehensive workflow for tumor image classification using Convolutional Neural Networks (CNNs) and transfer learning. The project includes custom CNN models and experiments with popular pretrained architectures (VGG16, ResNet50, EfficientNetB0), with augmentation, hyperparameter tuning, and robust class balancing for medical imaging datasets.

Project Overview
The workflow prepares clinical brain tumor image datasets, organizes folders for training/validation/testing, and applies preprocessing and augmentation techniques suitable for deep learning.

Multiple CNN architectures are used, including custom models and pretrained networks (VGG16, ResNet50, EfficientNetB0) with transfer learning and fine-tuning.

Models are trained to classify images into tumor types such as pituitary tumor, meningioma tumor, glioma tumor, and "no tumor" control samples.

Main Steps
Loads and preprocesses medical image data from organized directories, using Keras generators for augmentation and normalization.

Computes class weights to address dataset imbalance, and integrates these weights during model training for fair learning results.

Implements data augmentation (flip, rotation, zoom, contrast) to improve generalization and reduce overfitting.

Trains CNNs with early stopping and learning rate scheduling, iteratively fine-tuning trainable layers to optimize validation accuracy.

Experiments with freezing/unfreezing base layers and customizes classification heads tailored to the dataset.

Evaluates performance using cross-validated test sets, tracking accuracy and loss progression across epochs.

Results and Evaluation
Achieves improved test accuracy and validation metrics after fine-tuning and class weight balancing (notable increases when unfreezing and lowering learning rates).

Compares results of different architectures and configurations, showing model performance with and without augmentation, as well as baseline versus fine-tuned transfer learning.

