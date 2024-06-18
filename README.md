
# Malaria Cell Detection using CNN

This repository contains a project for detecting malaria-infected cells using a Convolutional Neural Network (CNN). The project includes data preprocessing, model training, and a web application for predicting whether a given cell image is infected with malaria or not.

## Table of Contents
- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
  - [Model Training](#model-training)
  - [Web Application](#web-application)

## Introduction

Malaria is a life-threatening disease caused by parasites that are transmitted to people through the bites of infected female Anopheles mosquitoes. Early detection of malaria is crucial for effective treatment. This project aims to automate the detection of malaria-infected cells using a deep learning model, specifically a Convolutional Neural Network (CNN).

## Project Structure

The repository is structured as follows:

```
.
├── Healthy.png                     # Example of a healthy cell image
├── Not Healthy.png                 # Example of an infected cell image
├── Malaria Cell Detection using CNN.ipynb  # Jupyter notebook for model training and evaluation
├── main_app.py                     # Flask web application for deploying the model
├── malaria_cell_detection.h5       # Trained CNN model
├── requirements.txt                # List of required Python packages
└── README.md                       # Project README file
```

## Installation

To run this project locally, follow these steps:

1. **Clone the repository**
    ```bash
    git clone https://github.com/yourusername/malaria-cell-detection.git
    cd malaria-cell-detection
    ```

2. **Create a virtual environment**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the required packages**
    ```bash
    pip install -r requirements.txt
    ```

## Usage

### Model Training

To train the model, open the Jupyter notebook `Malaria Cell Detection using CNN.ipynb` and follow the steps. The notebook includes data loading, preprocessing, model architecture, training, and evaluation.

### Web Application

To run the web application for predicting cell images, use the following command:

```bash
python main_app.py
```

The application will be accessible at `http://127.0.0.1:5000/`. You can upload a cell image to check whether it is infected with malaria.

### Example Images

- `Healthy.png`: Example of a healthy cell.
- `Not Healthy.png`: Example of an infected cell.

## Model Training

The Jupyter notebook `Malaria Cell Detection using CNN.ipynb` contains the entire workflow for training the CNN model. It includes:

1. **Data Loading**: Loading the dataset of cell images.
2. **Data Preprocessing**: Normalizing and augmenting the images.
3. **Model Architecture**: Defining the CNN architecture.
4. **Model Training**: Training the CNN on the dataset.
5. **Model Evaluation**: Evaluating the model's performance on the validation set.
6. **Saving the Model**: Saving the trained model as `malaria_cell_detection.h5`.

## Web Application

The web application is built using Flask. It allows users to upload a cell image and get a prediction on whether the cell is infected with malaria. The application uses the trained model (`malaria_cell_detection.h5`) to make predictions.

