# Email/SMS Spam Classifier

A machine learning project to classify email and SMS messages as spam or not spam using Natural Language Processing (NLP) techniques and various classification algorithms. The project includes a Streamlit web app for easy interaction.

## Overview
This project aims to classify messages as spam or not spam using machine learning techniques. The model is built and evaluated using various metrics, and a Streamlit web application is developed for user interaction.
![image](https://github.com/user-attachments/assets/1bb85616-483e-41c2-9190-a493b98685ec)
### Non-Spam Messages
![image](https://github.com/user-attachments/assets/513c85e4-4936-465e-bc77-0288cdef6cde)
### Spam Messages
![image](https://github.com/user-attachments/assets/26525d62-6ebf-4026-997b-df917fef570b)

## Dataset
The dataset used for this project is the SMS Spam Collection Dataset, which is available at UCI Machine Learning Repository.
Link: https://archive.ics.uci.edu/dataset/228/sms+spam+collection


## Installation
1. Clone the repository:
```bash
git clone https://github.com/rahulkumarmmmut/sms-spam-classifier.git
cd sms-spam-classifier
```
2. Create a virtual environment and activate it:
```bash
python -m venv env
source env/bin/activate  # On Windows use `env\Scripts\activate`
```
3. Install the required packages:
```bash
pip install -r requirements.txt
```
4. Download NLTK data:
```bash
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```

## Model Building
### Data Cleaning
1. Dropped unnecessary columns.
2. Renamed columns for clarity.
3. Encoded target labels.
4. Removed duplicate entries.
### Exploratory Data Analysis (EDA)
1. Visualized the distribution of spam and ham messages.
2. Analyzed message length, word count, and sentence count.
3. Created histograms and pair plots for deeper insights.
### Data Preprocessing
1. Converted text to lowercase.
2. Tokenized the text.
3. Removed special characters, stop words, and punctuation.
4. Applied stemming to reduce words to their root form.
### Model Building
1. Used CountVectorizer and TfidfVectorizer for text vectorization.
2. Scaled the features using MinMaxScaler.
3. Built models using GaussianNB, MultinomialNB, and BernoulliNB.
### Evaluation
1. Evaluated models using accuracy, confusion matrix, and precision score.
2. Chose the best-performing model for deployment.

## App Development
Developed a Streamlit web application with the following features:

1. Text area for inputting messages.
2. Button to trigger prediction.
3. Display of the prediction result (Spam or Not Spam).

## Usage
1. Run the Streamlit app:
```bash
streamlit run app/app.py
```
2. Open your web browser and go to http://localhost:8501.
3. Enter a message in the text area and click the "Predict" button to see the result.

## Future Work
1. Improve the model by trying different algorithms and hyperparameter tuning.
2. Enhance the web app with more features and a better UI.
3. Deploy the app on a cloud platform for wider accessibility.


## License

This project is licensed under the MIT License. See the LICENSE file for details.
