# SMS-Spam-Classification
Project Overview
This project aims to build a machine learning model to classify SMS messages as either spam or ham (non-spam). The project involves data exploration, feature engineering, model building, and evaluation. The final model can predict whether a given SMS message is spam or ham, using techniques like Naive Bayes and Decision Tree Classifiers.

Table of Contents
Project Overview
Dataset
Project Workflow
1. Importing Required Libraries
2. Loading and Exploring the Dataset
3. Label Encoding
4. Visualizing Imbalanced Dataset (Spam vs. Ham)
5. Handling Imbalanced Dataset Using Oversampling
6. Feature Engineering
7. Data Cleaning and Preprocessing
8. TF-IDF Vectorization
9. Model Building and Evaluation
10. Custom Function for Predicting Spam Messages
Results
Installation
Usage
Future Work
Contributing
License
Dataset
The dataset used in this project is a collection of SMS messages labeled as either "ham" (non-spam) or "spam". The data is loaded from a text file where each message is labeled and tab-separated.

Project Workflow
1. Importing Required Libraries
We start by importing essential libraries like Pandas, NumPy, Matplotlib, Seaborn, and NLTK for data manipulation, visualization, and natural language processing.

2. Loading and Exploring the Dataset
The dataset is loaded and initially explored to understand its structure. We look at the first few rows and get a summary of the data.

3. Label Encoding
The labels ("ham" and "spam") are converted into numerical values (0 and 1) to prepare for model training.

4. Visualizing Imbalanced Dataset (Spam vs. Ham)
We visualize the dataset to see the distribution of spam vs. ham messages, highlighting the imbalance in the data.

5. Handling Imbalanced Dataset Using Oversampling
To address the class imbalance, we oversample the spam messages to create a balanced dataset.

6. Feature Engineering
We create new features:

Word Count: Number of words in each SMS.
Currency Symbol Presence: Whether the message contains currency symbols.
Number Presence: Whether the message contains numeric characters.
7. Data Cleaning and Preprocessing
Text data is cleaned by removing special characters, stopwords, and numbers. Lemmatization is applied to reduce words to their base forms.

8. TF-IDF Vectorization
We use TF-IDF vectorization to convert the cleaned text into numerical features for model training.

9. Model Building and Evaluation
We train two models:

Naive Bayes Model
Decision Tree Model
Both models are evaluated using metrics like accuracy, precision, recall, and F1-score. Confusion matrices are visualized to understand the models' performance.

10. Custom Function for Predicting Spam Messages
A custom function is created to predict whether a given SMS message is spam or ham using the trained Decision Tree model.

Results
The models perform well, with the Naive Bayes model showing strong results. The Decision Tree model is also effective but has room for improvement. The accuracy of the models varies, but the overall ability to classify spam is robust.

Installation
To run this project locally, follow these steps:

Clone the repository:
bash
Copy code
git clone https://github.com/your-username/SMS-Spam-Detection.git
Navigate to the project directory:
bash
Copy code
cd SMS-Spam-Detection
Install the required packages:
Copy code
pip install -r requirements.txt
Usage
Run the Jupyter notebook or Python script to load the dataset, process the data, and train the models.
Use the predict_spam() function to classify any new SMS messages as spam or ham.
Future Work
Experiment with more advanced models like Random Forest or SVM.
Apply more sophisticated techniques for handling class imbalance.
Explore additional feature engineering techniques to improve model accuracy.
Contributing
Contributions are welcome! Please fork the repository and submit a pull request.

License
This project is licensed under the MIT License.
