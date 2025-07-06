# Fake_News_Detection
📰 Fake News Detection using NLP
📘 Project Overview
This project aims to classify news articles as real or fake using Natural Language Processing (NLP) techniques. The 'Fake News Dataset (Kaggle)' dataset was used for this analysis.
🔄 Steps Taken
1.	1. Data Loading and Preparation:
Loaded and combined the True.csv and Fake.csv files from the dataset. A subset of 2000 articles (1000 real and 1000 fake) was used for this analysis to expedite processing.
2.	2. Data Preprocessing:
Cleaned and preprocessed the text data by combining the 'title' and 'text' columns, converting text to lowercase, removing punctuation and stop words, and applying stemming using NLTK.
3.	3. Feature Extraction:
Used TF-IDF (Term Frequency-Inverse Document Frequency) to convert the preprocessed text data into numerical features. A TfidfVectorizer with max_features=5000 was used.
4.	4. Model Training:
A Logistic Regression model was trained on the TF-IDF features. The data was split into training (80%) and testing (20%) sets.
5.	5. Model Evaluation:
The model was evaluated using accuracy and a classification report.
📊 Results
The Logistic Regression model achieved an accuracy of 95.5% on the test set.
The classification report provides further details on precision, recall, and f1-score for both 'fake' and 'real' classes.
📈 Visualizations
Below are the visualizations for model performance and word distributions:
• Confusion Matrix
![confusion_Fake](https://github.com/user-attachments/assets/da15acb0-28c2-4cea-9507-2f13f824f21c)

• Precision-Recall-F1 Bar Chart
![Distribution](https://github.com/user-attachments/assets/55726dac-c012-4e37-a8d6-9e7bbabef488)

• Word Cloud of Real vs. Fake News
![wordcloud_fake](https://github.com/user-attachments/assets/12d08bcd-d4e0-4965-ab44-084a7f619362)

*(Add visualizations such as confusion matrix, word clouds, and TF-IDF feature importance plots here)*
🔮 Future Work
•	Experiment with different classifiers like Random Forests, SVM, or deep learning models.
•	Use more sophisticated text preprocessing like lemmatization and named entity recognition.
•	Incorporate metadata (e.g., author, publication date) for enhanced prediction.
•	Deploy the model as a web app using Flask or Streamlit.
