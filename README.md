# Debias-Racial-Bias-Using-GNN
# Recidivism Prediction with Graph Neural Networks

This project demonstrates the use of Graph Neural Networks (GNN) for predicting recidivism using various features from a recidivism dataset. The model is implemented using PyTorch and PyTorch Geometric.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Data Preparation](#data-preparation)
- [Training and Evaluation](#training-and-evaluation)
- [Results](#results)
- [References](#references)

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/cybercat37794/Debias-Racial-Bias-Using-GNN.git
   cd recidivism-gnn

python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`

pip install -r requirements.txt
2. Create and activate a virtual environment:

sh
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
3. Install the required packages:

sh
pip install -r requirements.txt
## Usage
Ensure your train and test datasets are available as CSV files.

Modify the file paths in the script to point to your dataset files.

Run the training script:

sh
python train.py
The model will be trained, and the metrics will be displayed and plotted.

## Project Structure
recidivism-gnn/
├── data/
│   ├── recidivism_train.csv
│   ├── recidivism_test.csv
├── src/
│   ├── train.py
├── README.md
├── requirements.txt

## Data Preparation
Load the train and test datasets from CSV files.

Encode categorical variables if not already encoded.

Extract features and labels for both train and test datasets.

Create nodes and edges based on specific criteria to form the graph structure.

## Training and Evaluation
The GNN model is implemented using GCNConv layers from PyTorch Geometric.

The model is trained using the Adam optimizer and Negative Log-Likelihood loss function.

Training and evaluation metrics such as accuracy, precision, recall, and F1 score are computed and plotted over epochs.

## Results
The training and evaluation metrics are plotted to provide a visual representation of the model's performance over epochs.
