# Heart-Stroke-Prediction-Using-ML-Application

## Overview
This is an end-to-end machine learning application for predicting the risk of stroke using a Flask backend, React frontend, and a trained machine learning model. The project integrates data preprocessing, model training, and deployment to provide users with a seamless experience.

---

## Features
- User-friendly React-based frontend interface.
- Flask API backend to serve the ML model predictions.
- Trained model for predicting stroke risk.
- Handles user inputs for age, gender, glucose levels, and smoking status.
- RESTful API for prediction endpoint.

---

## Tech Stack
### Backend
- **Flask**: For building RESTful APIs.
- **Flask-CORS**: To enable cross-origin requests.
- **Joblib**: For loading the pre-trained model.
- **Pandas**: For data handling and preprocessing.

### Frontend
- **React**: For building the user interface.
- **CSS**: For styling the application.

### Machine Learning
- **Scikit-learn**: For training the stroke prediction model.
- **Joblib**: For model serialization and loading.


---

## Prerequisites
- Python 3.7+
- Node.js 16+
- pip (Python package manager)

---

## Setup
### 1. Backend Setup
1. Navigate to the `backend/` directory:
   ```bash
   cd backend
   ```
2. Install required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Start the Flask server:
   ```bash
   python app.py
   ```

The backend server will start at `http://localhost:5000`.

### 2. Frontend Setup
1. Navigate to the `react-app/` directory:
   ```bash
   cd react-app
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the React development server:
   ```bash
   npm start
   ```

The React app will start at `http://localhost:3000`.

---

## API Endpoints
### POST `/predict`
- **Description**: Predicts stroke risk based on input data.
- **Request Body** (JSON):
  ```json
  {
    "age": 45,
    "gender": "Male",
    "avg_glucose_level": 120.5,
    "smoking_status": "Never Smoked"
  }
  ```
- **Response** (JSON):
  ```json
  {
    "stroke": 1
  }
  ```

---

## Results
The trained machine learning model achieved the following performance metrics:
- **Accuracy**: 91%
- **Precision**: 88%
- **Recall**: 85%
- **F1 Score**: 86%

---

## Future Enhancements
- Integrate more features for prediction.
- Deploy the app using Docker.
- Add user authentication.



## License
This project is licensed under the MIT License. See `LICENSE` for more details.

---

## Acknowledgments
- The dataset used for training the model was obtained from [Kaggle](https://www.kaggle.com/).
- Inspired by the YouTube tutorial by DataScience.
