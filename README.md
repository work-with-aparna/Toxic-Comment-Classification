# Toxic Comment Classification

This repository contains the implementation of a **Toxic Comment Classification** model that predicts the presence of different types of toxicity in online comments. The project utilizes Natural Language Processing (NLP) techniques and machine learning models to classify comments into multiple toxicity categories.

## Dataset
The dataset used for this project is sourced from the **Jigsaw Toxic Comment Classification Challenge** on Kaggle. It consists of online comments labeled with six different types of toxicity:
- **toxic**
- **severe_toxic**
- **obscene**
- **threat**
- **insult**
- **identity_hate**

## Approach

### 1. Preprocessing
- Tokenization and Lemmatization
- Removal of stopwords and special characters
- Conversion of text to lowercase
- Embedding extraction using **GloVe (Global Vectors for Word Representation)**
- Averaging the GloVe vectors to obtain fixed-length representations (25-length embedding vectors)

### 2. Model Training
- Multi-label classification setup with five output categories
- Various ML models tested, including Logistic Regression, Random Forest, and Neural Networks
- Evaluation using **Precision, Recall, F1-score, and AUC-ROC**

### 3. Results and Insights
- Performance comparison of different models
- Hyperparameter tuning for optimization
- Discussion of misclassifications and potential improvements

## Repository Structure
```
|-- Advanced Models.ipynb    # Jupyter Notebook for advanced models
|-- Basic Models.ipynb       # Jupyter Notebook for basic models
|-- sample_submission.csv    # Sample submission file
|-- train.csv                # Training dataset
|-- test.csv                 # Test dataset
|-- README.md                # Project documentation
```

## Installation
To set up the project environment, follow these steps:

1. Clone the repository:
   ```
   git clone https://github.com/work-with-aparna/Toxic-Comment-Classification.git
   cd Toxic-Comment-Classification
   ```

2. Create a virtual environment and activate it:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```


## Usage
To preprocess the dataset and train the model, run:
```bash
python src/Basic Models.ipynb
python src/Advanced Models.ipynb
```

## Future Work
- Experimenting with Transformer-based models like BERT
- Deploying the model as a web API
- Improving handling of imbalanced labels

## License
This project is licensed under the MIT License.
