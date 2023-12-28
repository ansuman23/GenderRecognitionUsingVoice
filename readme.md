The Project-Work on “GENDER RECOGNITION USING VOICE” introduces a ML-based 
recognition system that can be used to recognize the gender of a person (Male/Female) using 
his/her voice. 
The project is a beginner-friendly exploration of machine learning concepts and their 
application in a real-world scenario. It provides a foundation for understanding how voicebased systems can be trained to recognize certain patterns. 

**METHODOLOGY **

Data Collection: Audio files of male and female voices are collected from various online 
platforms and general survey among colleagues in .wav format. 
Feature Extraction: Librosa library is used to extract acoustic features using MFCC (MelFrequency Ceptral Coefficients) of each audio files. 
Preparation of dataset: Both male and female audio features, each containing features 
like mean_frequency, modindex upto 10 features, were put into a same dataset of .csv 
extension. 
Data Preprocessing and labelling: All those input data features were normalized to a 
value between 0 and 1 and output features were labelled as 1 for male and 0 for female. 
Splitting the dataset: The dataset is accessed using Pandas library in dataframe format and 
splitted into training data (80%) and test data (20%) using train_test_split function from 
sklearn library. 
Model selection and training: Four classifiers i.e. Random Forest, SVM, Logistic 
Regression, and Decision Tree were used to train and model the datas 
Model Evaluation: Performance evaluation metrics such as accuracy, f1-score, r2-score, 
mean_squared_error, and confusion matrix was calculated for each classifier mode 
Model Validation: Model is fed with custom audio file either in recorded(.wav) format or 
live recording through SoundDevice library to classify new audio as male or female. 
User Interface: A graphical user interface is built with tkinter library which displays 
buttons for recording/uploading audio file and show the classification result. 

Model Training Algorithms Used:
1. Random Forest Classifier
2. Support Vector Machine
3. Decision Tree Classifier
4. Logistic Regression

Model Performance Evaluation:
Accuracy of model in cases of Random Forest Classifier, Logistic Regression and SVM comes nearly same. So for choosing the right classifier for model validation we go for ROC/AUC curve analysis.

AUC(Area under Curve) comes to be higher in case of Random forest Classifier and hence it was chosen for final model validation using Custom testing of voice to classify the gender as Male or Female.

Model Validation:
![image](https://github.com/ansuman23/GenderRecognitionUsingVoice/assets/131350928/35d461d2-6eae-4d7d-a642-51e5cf76e6e1)
