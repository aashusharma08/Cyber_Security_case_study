# Cyber_Security_case_study
# README

## Network Intrusion Detection System using Random Forest and Logistic Regression

Welcome to the Network Intrusion Detection System (NIDS) project! This repository contains the implementation of a NIDS using machine learning techniques, specifically Random Forest and Logistic Regression. The system is designed to classify network activities as either normal or an attack, and further identify the type of attack.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Training and Evaluation](#model-training-and-evaluation)
  - [Binary Classification](#binary-classification)
  - [Multinomial Classification](#multinomial-classification)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Network Intrusion Detection Systems are essential for ensuring the security of computer networks. This project leverages machine learning algorithms to detect and classify network intrusions, enhancing network security by identifying malicious activities in real-time.

## Features

- Binary classification to detect whether network activity is normal or an attack.
- Multinomial classification to identify specific types of attacks.
- Uses Logistic Regression for binary classification and Random Forest for multinomial classification.
- Handles imbalanced data using the SMOTE technique.
- Provides high accuracy in detecting and classifying network intrusions.

## Installation

To get started with this project, follow these steps:

1. **Clone the repository**:
    ```sh
    git clone <repository_url>
    ```

2. **Navigate to the project directory**:
    ```sh
    cd <project_directory>
    ```

3. **Install the required dependencies**:
    ```sh
    pip install -r requirements.txt
    ```

Make sure to replace `<repository_url>` and `<project_directory>` with the actual repository URL and directory name.

## Usage

1. **Prepare the dataset**: Ensure that the dataset files are in the project directory. The dataset files include:
    - Data_of_Attack_Back.csv
    - Data_of_Attack_Back_BufferOverflow.csv
    - Data_of_Attack_Back_FTPWrite.csv
    - Data_of_Attack_Back_GuessPassword.csv
    - Data_of_Attack_Back_Neptune.csv
    - Data_of_Attack_Back_NMap.csv
    - Data_of_Attack_Back_Normal.csv
    - Data_of_Attack_Back_PortSweep.csv
    - Data_of_Attack_Back_RootKit.csv
    - Data_of_Attack_Back_Satan.csv
    - Data_of_Attack_Back_Smurf.csv

2. **Run the script**:
    ```sh
    python nids.py
    ```

3. **View the results**: The script will print the classification reports and confusion matrices for both binary and multinomial classification models.

## Dataset

The dataset consists of various types of network activities labeled as normal or different types of attacks. Each file corresponds to a specific type of network activity, either normal or a particular attack type.

## Model Training and Evaluation

### Binary Classification

- **Objective**: Classify network activities as either normal or an attack.
- **Algorithm**: Logistic Regression.
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, Confusion Matrix.

### Multinomial Classification

- **Objective**: Identify the specific type of attack.
- **Algorithm**: Random Forest.
- **Evaluation Metrics**: Accuracy, Precision, Recall, F1-Score, Confusion Matrix.

## Results

The models demonstrate high accuracy and performance in detecting and classifying network intrusions. The Logistic Regression model for binary classification achieved an accuracy of 99%, while the Random Forest model for multinomial classification achieved nearly 100% accuracy.

## Contributing

We welcome contributions to improve this project! If you would like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a pull request.

For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License.

