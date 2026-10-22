# ♻️ EcoSort: AI-Powered Waste Management Assistant

## Project Overview

EcoSort is an AI-powered waste management assistant designed to help users identify waste materials and understand how to dispose of them correctly.

The project combines image classification, text classification, and policy-based information retrieval to support smarter waste sorting and recycling decisions.

This project was developed as part of a Data Science summative lab focused on neural networks and similar machine learning models.

## Problem Statement

Incorrect waste sorting can make recycling more difficult and increase the amount of waste sent to landfills. People may also be unsure how to dispose of different materials correctly.

EcoSort explores how machine learning and natural language processing can help users identify waste and access relevant disposal guidance.

## Project Objectives

- Classify waste materials from uploaded images.
- Predict waste categories from written descriptions.
- Retrieve relevant recycling instructions from waste management policy documents.
- Integrate the components into a unified waste management assistant.
- Evaluate model performance using test data and sample cases.

## Technologies Used

- **Python** — data processing and model development
- **Pandas and NumPy** — data exploration and manipulation
- **TensorFlow/Keras** — image classification
- **MobileNetV2** — transfer learning for waste image recognition
- **Scikit-learn** — text classification, TF-IDF vectorization, and similarity calculations
- **Transformers** — pretrained language model tooling
- **Jupyter Notebook** — experimentation and documentation
- **Git and GitHub** — version control and project sharing

## Datasets

The project uses three main data sources:

| Dataset | Purpose |
|---|---|
| RealWaste image dataset | Training and evaluating the image classification model |
| `waste_descriptions.csv` | Training and evaluating the text classification model |
| `waste_policy_documents.json` | Providing policy information for recycling instruction retrieval |

The waste descriptions and policy documents were generated for the project to simulate waste management scenarios.

**Note:** The RealWaste image dataset is not included in this repository. Download it separately and place it in the directory structure expected by the notebook.

## Project Workflow

### 1. Data Exploration and Preparation

- Explored the image, text, and policy datasets.
- Prepared images for model training.
- Processed text descriptions and extracted numerical features.
- Prepared policy documents for information retrieval.

### 2. Image Classification

A pretrained MobileNetV2 model was used through transfer learning to classify waste images into their respective categories.

The workflow included image preprocessing, model training, validation, and fine-tuning.

### 3. Text Classification

A Multinomial Naive Bayes model was trained to predict waste categories from written descriptions.

TF-IDF vectorization converted text into numerical features that the classifier could use.

### 4. Recycling Instruction Retrieval

A policy retrieval component was developed using TF-IDF document representations and cosine similarity.

Given a query, the system identifies relevant policy information and presents the retrieved content as recycling guidance. This helps ground the instructions in the available reference documents.

### 5. Integrated Assistant

The individual components were connected into a unified workflow that accepts either a waste image or a written description, predicts the waste category, and retrieves relevant disposal guidance.

## Model Results

The following results were observed during experimentation:

| Component | Reported result |
|---|---:|
| Image classification | Approximately 81.04% test accuracy |
| Best image-model validation accuracy during fine-tuning | 83.62% |
| Text classification | 99.60% test accuracy |

These results reflect the evaluated datasets and experimental setup. They do not guarantee the same performance on real-world waste images or descriptions.

## Project Structure

```text
ecosort-summative-lab/
│
├── waste_management_summative.ipynb
├── waste_descriptions.csv
├── waste_policy_documents.json
├── README.md
└── .gitignore
```

The RealWaste image dataset is stored separately and excluded from version control.

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/margaretkarugu39/ecosort-summative-lab.git
```

### 2. Navigate to the project directory

```bash
cd ecosort-summative-lab
```

### 3. Set up the environment

Create and activate a Python environment, then install the packages required by the notebook.

For example:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn tensorflow transformers torch jupyter
```

Package versions may need to be adjusted to match the notebook and your Python environment.

### 4. Prepare the image dataset

Download the RealWaste dataset, extract it, and arrange its class folders according to the directory paths used in the notebook.

### 5. Open the notebook

```bash
jupyter notebook waste_management_summative.ipynb
```

Run the notebook cells in order. Some steps may require downloading pretrained model weights or other resources.

## Limitations and Future Improvements

- Evaluate image predictions across all classes using a confusion matrix and additional metrics.
- Investigate waste categories that are frequently misclassified.
- Test the models on more diverse, real-world waste descriptions and images.
- Improve retrieval relevance and evaluate the accuracy of recycling guidance.
- Explore stronger text models and more advanced retrieval methods.
- Develop a user-friendly web interface for practical use.

## Conclusion

EcoSort demonstrates how computer vision, text classification, and policy-based retrieval can be combined to support waste identification and recycling guidance.

The project provided practical experience in data preparation, transfer learning, natural language processing, model evaluation, and integrating multiple machine learning components into one application.

## Author

**Margaret Karugu**

Data Science Student | Aspiring Data Analyst

GitHub: [@margaretkarugu39](https://github.com/margaretkarugu39)

Project repository: [EcoSort Waste Management Assistant](https://github.com/margaretkarugu39/ecosort-summative-lab)
