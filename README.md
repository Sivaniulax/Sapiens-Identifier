# Sapiens-Identifier
Sapiens-Identifier is an end to end Machine learning project which is a classifies human face with model Accuracy of 95%.
 
 Data Collection:
 In this project, the data(images) are web scrapped from google for few sports celebraties and by Fatkun Batch download extension of Google.
 
 Data Cleaning and Preparation:
 In cleaning part, OpenCV(haar cascade) is used for removing images which has less information (like., no eyes, turned position, without face, etc...) to reduce manual work and face is cropped and stored in separate destination for further use. Then manual review or elimination of data is performed to avoid misclassification. Then the images is subjected to Wavelet Transform, which is the most successfull transform method to produce information like length of the forehead, width of the nose, size of the eye, etc... it's in Black and white images. As performing Classification with Colour image is difficult, therefore the image are converted into grey scale images and  transformed using Wavelet Transform.
 
 Model Building and deployment and frontend:
 The Model is trained with Machine learning Algorithms like SVM, RandomForest Algorithm and Logistic Regression with accuracies 83%, 64% and 94%, hence best model is built using Logistic Regression, but here a good model is built with SVM. In Addition to that the model is deployed using Flask and frontend is designed and attached to pickle file through pipeline by HTML, CSS and Javascript.
 
 
Libraries Used: Numpy, (OpenCV) cv2,  matplotlib, (matplotlib) pyplot, (Wavelet Transform) pywt, os, shutil, sklearn.svm, sklearn.preprocessing, sklearn.model_selection, sklearn.pipeline, sklearn.metrics, sklearn.ensemble(RandomForestClassifier), sklearn.linear_model(LogisticRegression), sklearn.pipelin(make_pipeline), sklearn.model_selection(GridSearchCV), seaborn, joblib (save model).


OVERVIEW:
![image](https://user-images.githubusercontent.com/91459697/204022862-db05b56a-4d7f-4719-a26e-da8026c78b46.png)

PREDICTION:
![image](https://user-images.githubusercontent.com/91459697/204022981-1a8e0cac-eee6-4ca3-9edf-e2f4a2648658.png)

![image](https://user-images.githubusercontent.com/91459697/204023048-b212aece-232e-456b-85b1-b07c0a608192.png)
