# Drone RF Signal Classification 2023

This repository contains the code and models for the project "Drone RF Signal Classification 2023," which focuses on utilizing machine learning techniques to classify RF signals emitted by drones. The goal is to create a system that can accurately identify different drone signatures in noisy environments.

## Project Structure

- `SNR_stats.csv` - Contains signal-to-noise ratio statistics of the RF signals.
- `balanced_feature_data.csv` - The balanced dataset after feature engineering for model training.
- `class_stats.csv` - Statistics on the classification performance of different models.
- `extracted-features.ipynb` - Jupyter notebook for feature extraction from raw signal data.
- `feature_data.csv` - The raw feature data extracted from RF signals.
- `knn_model.joblib` - Serialized K-Nearest Neighbors model trained on the dataset.
- `train.ipynb` - Jupyter notebook containing the training pipeline for the models.
- `xgboost_model.joblib` - Serialized XGBoost model trained on the dataset.

## Installation

Before running the project, ensure you have Python 3.8+ and the following packages installed:
- pandas
- scikit-learn
- xgboost
- jupyter

You can install the dependencies with the following command:

```bash
pip install pandas scikit-learn xgboost jupyter
```

##Usage

To start working with the project, clone the repository to your local machine using:

```bash
git clone https://github.com/lumenalux/drone-rf-signal-classification-2023.git
```

To extract features from the raw signal data, run the `extracted-features.ipynb` notebook.

For training the models with the preprocessed dataset, execute the `train.ipynb` notebook.

## Models


Two main machine learning models are used:

-   K-Nearest Neighbors (KNN): A simple yet effective algorithm for classification tasks.
-   XGBoost: An advanced gradient boosting machine learning framework that is highly scalable and provides better accuracy.
