OVERVIEW OF THE PROJECT

This project is dedicated to the creation of a machine learning model to classify emails into spam and ham categories. Using text processing techniques together with Logistic Regression, the system learns patterns from email content and predicts the category for new incoming emails.



TECHNOLOGIES USED

Python
NumPy
Pandas
Scikit-learn
TF-IDF Vectorization
Logistic Regression




DATASET

The data used in this project is contained in a CSV file, mail_data.csv, which has two columns:
Category-spam or ham
Message - the text of the email
Missing values were replaced with empty strings for consistency.




STEPS IN THE PROJECT

1. Importing Dependencies
All the needed libraries for loading, preprocessing, feature extraction, model training, and evaluation are imported here.
2. Data Collection & Pre-processing
The dataset is loaded into a Pandas DataFrame.
Null values are replaced with empty strings.
Categories are encoded as
spam → 0
ham → 1
3. Splitting the Dataset
The data is divided into the training set and the testing set in the ratio of 80%–20%, respectively, by utilizing the function train_test_split().
4. Feature Extraction
The TF-IDF Vectorizer transforms email text into numerical feature vectors understandable to the model.
5. Model Training
A Logistic Regression model is trained on the TF-IDF features by using the training data.
6. Model Evaluation
The model's accuracy is verified on:
Training data
Testing data
Using accuracy_score().
7. Predictive System
A sample email is passed through the trained model to predict whether it is:
Ham (1)
Spam (0)
This concludes the real-time classification part of the project.



HOW TO RUN THE PROJECT

1. Upload mail_data.csv to your working directory (e.g., Google Colab).
2. Execute the Python script in steps.
3. Once trained, you can try inserting your own email text into the input area to check the prediction.
Complete the statements.





Output

Accuracy of the model on training and test data
Prediction for any given email
Final output displayed as “Spam mail” or “Ham mail”



CONCLUSION

Spam and ham emails can be effectively singled out by the model using TF-IDF features with logistic regression. The model can be improved further with more sophisticated algorithms or additional data.
