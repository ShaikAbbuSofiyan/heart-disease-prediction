❤️ Heart Disease Prediction App

This project is a Streamlit web application for predicting the risk of heart disease based on user inputs such as age, blood pressure, cholesterol, and other medical attributes.
It uses a Support Vector Machine (SVM) model trained on heart disease datasets, along with feature scaling and one-hot encoded categorical variables.

🚀 Features

Interactive Streamlit UI for user-friendly inputs.

Accepts medical features like:

Age

Sex

Chest pain type

Resting blood pressure

Cholesterol

Fasting blood sugar

Resting ECG results

Maximum heart rate

Exercise-induced angina

Oldpeak (ST depression)

ST slope

Pre-trained SVM model (SVM_heart.pkl) used for predictions.

MinMaxScaler (scaler.pkl) for feature scaling.

Dynamic column handling with columns.pkl for robust input matching.

Displays Low Risk or High Risk of heart disease.

📂 Project Structure
├── app.py                # Streamlit application (main code)
├── SVM_heart.pkl         # Trained SVM model
├── scaler.pkl            # Fitted scaler for preprocessing
├── columns.pkl           # Expected feature columns
├── requirements.txt      # Dependencies
└── README.md             # Project documentation

⚙️ Installation & Setup

Clone the repository

git clone https://github.com/ShaikAbbuSofiyan/heart-disease-prediction.git
cd heart-disease-prediction


Create a virtual environment (recommended)

python -m venv venv
source venv/bin/activate      # Linux/Mac
venv\Scripts\activate         # Windows


Install dependencies

pip install -r requirements.txt


Run the Streamlit app

streamlit run app.py

📦 Requirements

Your requirements.txt should include:

streamlit
pandas
numpy
scikit-learn
joblib

🧠 Model Training (Optional)

If you want to retrain the model:

Use a heart disease dataset (e.g., UCI Heart Disease dataset).

Perform preprocessing (encoding categorical variables, scaling, etc.).

Train an SVM model:

from sklearn.svm import SVC
model = SVC(probability=True)
model.fit(X_train, y_train)


Save artifacts:

import joblib
joblib.dump(model, "SVM_heart.pkl")
joblib.dump(scaler, "scaler.pkl")
joblib.dump(expected_columns, "columns.pkl")

🖥️ Demo

After running, the app will let you:

Enter medical attributes.

Click Predict.

Get instant feedback:
✅ Low Risk of Heart Disease
❌ High Risk of Heart Disease

🌐 Deployment

You can deploy this project on:

Streamlit Cloud

Heroku

Render

✨ Author

Developed by ShaikAbbuSofiyan
 🧑‍💻
Feel free to connect with me on LinkedIn [!LinkedIn](www.linkedin.com/in/shaik-abbu-sofiyan-1427a128b)
 or check out my other projects!
