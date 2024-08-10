# ESOL Graph Neural Network Model

## Overview

This project implements a Graph Neural Network (GNN) model to predict the water solubility of molecules using the ESOL (Estimated SOLubility) dataset. The model uses molecular graph structures to learn and predict solubility values.

## Purpose

The primary goal of this project is to demonstrate the application of Graph Neural Networks in predicting molecular properties, specifically water solubility. This model can be useful in various fields, including drug discovery, materials science, and chemical engineering.

## Dependencies

- Python 3.x
- PyTorch
- PyTorch Geometric
- RDKit
- NumPy
- Pandas
- Matplotlib
- Seaborn

## Model Architecture

The GNN model consists of:
- 3 Graph Convolutional Network (GCN) layers
- Global mean and max pooling
- A final linear layer for prediction

## Dataset

The model uses the ESOL dataset, which contains:
- SMILES representations of molecules
- Experimental water solubility values

## Usage

1. Data Preparation:
   - Convert SMILES to RDKit molecules
   - Extract molecular graph features

2. Model Training:
   - Initialize the GCN model
   - Train using MSE loss and Adam optimizer
   - Monitor training loss

3. Evaluation:
   - Predict solubility on test set
   - Visualize results using scatter plots

## Results

The model demonstrates the ability to predict water solubility with reasonable accuracy, as shown in the scatter plot of predicted vs. actual solubility values.

## Future Improvements

- Experiment with different GNN architectures (e.g., GAT, GraphSAGE)
- Implement cross-validation for more robust evaluation
- Explore hyperparameter tuning
- Incorporate additional molecular features

## References

- ESOL Dataset
- DeepFIndr
