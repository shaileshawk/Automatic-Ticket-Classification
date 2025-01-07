# Automatic-Ticket-Classification
# Automatic Ticket Classification Project

## Overview
The **Automatic Ticket Classification Project**, created by **Shailesh Patel**, a student of the Postgraduate Program in Machine Learning & Artificial Intelligence, aims to classify customer complaints based on products or services. This enables quick resolution of issues by mapping tickets to their respective categories.

## Objective
The goal is to build a model capable of:
- Analyzing and segregating customer complaint tickets into five categories:
  - Credit Card / Prepaid Card
  - Bank Account Services
  - Theft/Dispute Reporting
  - Mortgages/Loans
  - Others
- Using **Topic Modeling** (via **NMF**) to identify patterns and classify tickets.
- Training supervised models (e.g., Logistic Regression, Decision Tree, or Random Forest) to classify new tickets.

## Dataset
- **Format:** JSON
- **Preparation:**
  - Convert JSON to a dataframe.
  - Perform text cleaning and preprocessing:
    - Lowercasing
    - Removing square-bracket text
    - Removing punctuation
    - Removing words with numbers
    - Lemmatization
    - POS tagging (retain only nouns)

## Methodology
1. **Data Preprocessing:**
   - Handle missing values.
   - Apply text normalization and cleaning techniques.
2. **Topic Modeling:**
   - Use **Non-Negative Matrix Factorization (NMF)** for clustering complaints.
   - Map topics to specific categories based on patterns.
3. **Model Training:**
   - Use the topic-labeled data to train supervised learning models.
4. **Model Evaluation:**
   - Evaluate performance using metrics such as accuracy, precision, recall, and F1 score.

## Libraries Used
- Python Core Libraries: `pandas`, `numpy`
- Visualization: `matplotlib`, `seaborn`
- Text Processing: `nltk`, `sklearn`
- Machine Learning Models: `sklearn`

## Results
- Successfully classified customer complaints into the predefined categories.
- Developed a pipeline for scalable and automated ticket classification.

## How to Run the Project
1. Install required libraries using:
   ```bash
   pip install -r requirements.txt
   ```
2. Run the provided Jupyter notebook:
   ```bash
   jupyter notebook AutomaticTicketClassification.ipynb
   ```
3. Follow the notebook steps to preprocess the data, build models, and visualize results.

## Future Work
- Enhance the classification accuracy by:
  - Experimenting with advanced models (e.g., Transformer-based models like BERT).
  - Leveraging additional labeled data.
- Deploy the model for real-time ticket classification.

## Author
**Shailesh Patel**  
Postgraduate Program in Machine Learning & Artificial Intelligence  

---
For any inquiries or collaborations, please reach out!
