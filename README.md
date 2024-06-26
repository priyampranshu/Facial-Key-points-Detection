
# Facial Key-points Detection

This repository contains the implementation of a deep learning model for detecting facial key-points in images. The project uses a Residual Neural Network (ResNet) for predicting the coordinates of key facial features.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Model Architecture](#model-architecture)
- [Data Augmentation](#data-augmentation)
- [Training and Evaluation](#training-and-evaluation)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation

1. Clone the repository:
 
    git clone https://github.com/yourusername/Facial-Key-points-Detection.git
    cd Facial-Key-points-Detection


2. Install the required dependencies:

    pip install -r requirements.txt


## Usage

1. Place the dataset file `KeyFacialPoints.csv` in the root directory of the project.
2. Run the Jupyter Notebook or Python script to process the data, train the model, and evaluate the results.

## Project Structure

- `data/`: Contains the dataset file `KeyFacialPoints.csv`.
- `notebooks/`: Jupyter Notebooks for data processing, model training, and evaluation.
- `scripts/`: Python scripts for data processing, model training, and evaluation.
- `models/`: Directory to save trained models.
- `requirements.txt`: List of dependencies required for the project.

## Model Architecture

The model uses a Residual Neural Network (ResNet) architecture, which includes:
- Convolutional blocks with batch normalization and activation layers.
- Identity blocks for maintaining the input dimensions.
- Average pooling and dense layers for the final output.

## Data Augmentation

The data augmentation techniques used in this project include:
- Horizontal flipping
- Vertical flipping
- Random brightness adjustment

## Training and Evaluation

The model is compiled and trained using the Adam optimizer with mean squared error loss. The training process includes:
- Splitting the data into training and testing sets.
- Normalizing the images.
- Using a checkpoint to save the best model based on validation loss.

## Results

The model is evaluated on the test set, and the accuracy and RMSE (Root Mean Squared Error) are reported. Additionally, the predicted key-points are visualized on sample test images.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.
