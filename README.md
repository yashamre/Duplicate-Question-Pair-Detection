# DisQuorNet: A Machine Learning Framework for Identifying Duplicate Question Pairs on Quora

## Project Overview

Quora, as a large online Q&A platform, faces the issue of duplicate questions. These duplicate queries clutter the platform, making it difficult for users to find valuable content and negatively impacting the user experience. **DisQuorNet** is a machine learning framework designed to identify and eliminate these duplicate question pairs, thereby enhancing Quora's content organization and user satisfaction.

## Purpose

The main goal of this project is to build a framework that uses **Natural Language Processing (NLP)** and **machine learning techniques** to accurately detect duplicate question pairs on Quora. The project addresses the following challenges:
- Processing a vast amount of data generated by users.
- Identifying semantically similar questions with different wording and phrasing.
- Using machine learning algorithms to enhance the accuracy of the detection system.

## Features

- **Text Processing and NLP:** Includes tokenization, stemming, and advanced word embedding techniques like **Bag of Words (BoW)**.
- **Machine Learning Models:** Utilizes algorithms such as **Random Forest**, **XGBoost**, **Logistic Regression**, and **Support Vector Machines (SVM)** for classifying question pairs as duplicates or non-duplicates.
- **Deep Learning Potential:** The project explores the use of **Siamese LSTM** networks to capture the nuances of sequential text data for enhanced accuracy in detecting similar questions.
- **User-friendly Interface:** A GUI using **Streamlit** that allows users to input pairs of questions or documents for real-time duplicate detection.

## Tools and Technologies

- **Programming Languages:** Python
- **Libraries and Frameworks:**
  - NLP: `nltk`, `Spacy`, `fuzzywuzzy`
  - Machine Learning: `Scikit-learn`, `XGBoost`
  - Data Processing: `Pandas`, `NumPy`
  - Visualization: `Matplotlib`, `Seaborn`
  - GUI: `Streamlit`
- **Dataset:** The project uses the **Quora Question Pairs dataset** from Kaggle.

## System Architecture

The proposed system architecture is composed of the following components:
1. **Preprocessing:** Clean and preprocess the dataset by tokenizing, stemming, and normalizing text.
2. **Feature Engineering:** Extract features like word counts, word shares, and semantic similarity using word embeddings.
3. **Model Training:** Train machine learning models on labeled datasets of question pairs, utilizing features like **TF-IDF**, **BoW**, and word embeddings.
4. **Duplicate Detection:** The trained model predicts whether input question pairs are duplicates or not.
5. **User Interface:** Users can input question pairs or upload documents for duplicate detection through the web interface.

## Project Structure

```
|-- data/                # Dataset for training and testing
|-- notebooks/           # Jupyter notebooks for experimentation
|-- src/                 # Python scripts for text processing and model building
|-- reports/             # Final reports and visualizations
|-- README.md            # Project documentation
|-- requirements.txt     # List of dependencies
```

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/DisQuorNet.git
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Streamlit app:
   ```bash
   streamlit run src/app.py
   ```

## Usage

### Running the Duplicate Detection

1. **Input Questions Manually:**
   Users can input two questions to check for similarity and detect if they are duplicates.

2. **Upload Text File:**
   Users can upload a text file containing multiple question pairs, and the system will analyze and detect duplicate questions.

3. **Upload Two Documents:**
   Users can upload two separate documents, and the system will identify similar question pairs between the two documents.

## Results

The model provides a high accuracy in detecting duplicate questions, with performance evaluated using:
- **Accuracy**
- **Precision**
- **Recall**
- **F1 Score**

Confusion matrices from **Random Forest** and **XGBoost** models show strong performance across test data.

## Future Work

- **Multilingual Support:** Expanding the framework to detect duplicate questions in multiple languages such as Hindi and Marathi.
- **Deep Learning Integration:** Implementing **Siamese LSTM** networks to improve the model's understanding of the context and meaning behind questions.
- **User Feedback Mechanism:** Allowing users to provide feedback on detected duplicate pairs to improve model accuracy.

## Contributions

We welcome contributions! If you'd like to collaborate, please fork the repository and submit a pull request with a clear description of the changes.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
