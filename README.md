🧬 Breast Cancer Prediction - Logistic Regression

📌 Overview

This project implements a Machine Learning model to classify breast cancer tumors as Cancerous (Malignant) or Not Cancerous (Benign).
The pipeline includes data preprocessing, EDA, model training, prediction system, and deployment using Flask with an HTML interface.


---

📊 Dataset

Source: Kaggle - Breast Cancer Dataset

Samples: 569 records

Features: 30 numeric features (e.g., radius, texture, smoothness)

Target Variable:

0 → Malignant (Cancerous)

1 → Benign (Not Cancerous)




---

⚙ Workflow

1. Data Loading

Downloaded dataset from Kaggle.

Loaded using pandas.



2. Data Preprocessing

Encoded target variable using LabelEncoder.

Split dataset: 80% training / 20% testing.

Applied StandardScaler for feature scaling.



3. Exploratory Data Analysis (EDA)

Visualized distribution of diagnosis (Malignant vs Benign).

Calculated correlation matrix between features.


4. Model Training

Applied Logistic Regression.

Achieved 97% accuracy.



5. Prediction System

Function accepts input features.

Outputs:

Cancerous (if malignant)

Not Cancerous (if benign).




6. Model Saving & Loading

Saved trained model using pickle.

Reloaded model for deployment.



7. Deployment

Built a Flask web application.

Integrated an HTML interface with supportive images/icons.

Users can input features and get prediction in real-time.





---

🧪 Results

Logistic Regression → 97% Accuracy

Prediction system works correctly on unseen data.

Flask App deployed successfully.



---

🚀 How to Run

1. Clone this repo:

git clone https://github.com/ali403624/Breast-Cancer-logistic-regression.


2. Install dependencies:

pip install -r requirements.txt


3. Run the Flask app:

python app.py


4. Open in browser:

http://127.0.0.1:5000/predict




---

📦 Requirements

Python 3.8+

pandas

numpy

scikit-learn

matplotlib

flask



---

📸 Screenshots

(

![Distribution of Diagnosis Plot](https://drive.google.com/file/d/1JzQqSCkbKr4a4uJWD-anJI61K9kcojek/view?usp=drivesdk)  
 
![Flask App](https://drive.google.com/file/d/1nGSigYKQ7B090mRO-yd3L2qU1pF3xwFU/view?usp=drivesdk)

![Flask App](https://drive.google.com/file/d/10FVcvBcqo6HIgbs64kIvHYdMb7foK5tY/view?usp=drivesdk)


---

✨ Future Work

Try other ML models (Random Forest, SVM) for comparison.

Hyperparameter tuning for better performance.

Deploy app to Heroku/Render for online access.
