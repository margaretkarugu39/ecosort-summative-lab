# EcoSort: AI-Powered Waste Management Assistant

## Project Overview

EcoSort is an AI-powered waste management assistant designed to help residents identify waste materials and receive appropriate recycling and disposal instructions.

## Project Objectives

- Classify waste materials from images using a Convolutional Neural Network (CNN).
- Classify waste descriptions using a text classification model.
- Retrieve relevant policy documents and generate recycling instructions using Retrieval-Augmented Generation (RAG).
- Integrate the models into a unified waste management assistant.
- Evaluate model performance and identify areas for improvement.

## Project Components

1. Dataset exploration and preparation
2. CNN-based image classification
3. Waste description classification
4. RAG-based recycling instruction generation
5. Integrated waste management assistant

## Datasets

- RealWaste image dataset
- Waste item descriptions in `waste_descriptions.csv`
- Waste management policies in `waste_policy_documents.json`

The image dataset is stored locally and excluded from this repository because of its size.

## Technologies

- Python
- Jupyter Notebook
- Pandas and NumPy
- Scikit-learn
- Deep learning frameworks
- Natural Language Processing
- Transformer models and document retrieval

## How to Run

1. Clone this repository.
2. Install the required dependencies.
3. Download or locate the RealWaste image dataset.
4. Ensure the datasets are stored in the locations expected by the notebook.
5. Open `waste_management_summative.ipynb` in VS Code or Jupyter Notebook.
6. Run the notebook cells in order.

## Project Status

In progress. Model implementations, evaluation results, and final documentation will be added as the project develops.
