# SMS Spam Detector


## Project Overview

This project implements SMS text classification using a pipeline with TF-IDF vectorization and Linear Support Vector Classification (SVC). The goal is to classify SMS messages as spam or non-spam (ham) based on their content. The project includes building a pipeline, splitting the data into training and testing sets, training the model, and deploying it via a Gradio app for user interaction.

## Preprocessing and Model Pipeline

The preprocessing and model pipeline involves the following steps:

1. **Data Loading and Splitting**: 
   - Load SMS data from a DataFrame (`sms_text_df`) containing 'text_message' and 'label' columns.
   - Split the data into training and testing sets using `train_test_split` from scikit-learn.

2. **Text Preprocessing**:
   - **TF-IDF Vectorization**: Convert text messages into numerical vectors using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. 
   
3. **Model Construction**:
   - **Linear Support Vector Classification (SVC)**: Build a pipeline that combines TF-IDF vectorization (`TfidfVectorizer`) with a Linear SVC classifier (`LinearSVC`). 

## Training the Model

- **Training**: Fit the pipeline model (`text_clf`) to the training data (`X_train` and `y_train`). This step involves learning the patterns and relationships between SMS messages and their corresponding labels (spam or ham).

## Deployment and Usage

- **Gradio App**: Once trained, the model can be deployed using Gradio to create an interactive app where users can input text and output is given on whether the text is Spam is not. 

## Improvements

Potential improvements include:
- Experimenting with different text preprocessing techniques to further enhance model performance.
- Tuning hyperparameters of both TF-IDF vectorization and SVC to optimize classification accuracy.
- Exploring alternative machine learning algorithms (e.g., Naive Bayes, Logistic Regression) to compare and improve model performance.

## Sources
- Tutors
- ChatGPT
- Classmates