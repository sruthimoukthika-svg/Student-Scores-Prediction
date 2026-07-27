# 🎓 Student Placement Predictor

A Machine Learning web application built with **Python**, **Streamlit**, and **Scikit-learn** that predicts whether a student is likely to be **Placed** or **Not Placed** based on their academic performance and study habits.

## 📌 Project Overview

This project uses a **Support Vector Machine (SVM)** classification model to predict a student's placement status. Users enter student information through a simple Streamlit interface, and the model provides an instant prediction.

This project demonstrates the complete machine learning workflow:
- Data preprocessing
- Model training
- Model saving using Joblib
- Deploying the model with Streamlit

---

## 🚀 Features

- Easy-to-use web interface
- Real-time placement prediction
- Machine Learning model using Support Vector Machine (SVM)
- Interactive input fields
- Instant prediction results

---

## 🛠️ Technologies Used

- Python
- Streamlit
- Pandas
- Scikit-learn
- Joblib

---

## 📂 Project Structure

```
Student-Placement-Predictor/
│
├── app.py                 # Streamlit application
├── SVM.pkl                # Trained SVM model
├── README.md              # Project documentation
└── dataset.csv            # Dataset (optional)
```

---

## 📊 Input Features

The model predicts placement using the following features:

| Feature | Description |
|----------|-------------|
| Study Hours | Average hours studied per day |
| Attendance | Attendance percentage |
| Sleep Hours | Average hours of sleep |
| Internet Usage | Daily internet usage (hours) |
| Assignments Completed | Number of assignments completed |
| Previous Score | Previous exam score |

---

## 🎯 Output

The model predicts one of two classes:

- ✅ Placed
- ❌ Not Placed

---

## ▶️ How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/student-placement-predictor.git
```

### 2. Navigate to the project folder

```bash
cd student-placement-predictor
```

### 3. Install the required libraries

```bash
pip install streamlit pandas scikit-learn joblib
```

### 4. Run the Streamlit app

```bash
streamlit run app.py
```

The application will open in your default web browser.

---

## 🧠 Machine Learning Model

The project uses a **Support Vector Machine (SVM)** classifier.

After comparing multiple machine learning algorithms, the SVM model achieved the best performance for this dataset and was saved as:

```
SVM.pkl
```

The trained model is loaded using Joblib:

```python
model = joblib.load("SVM.pkl")
```

---

## 💻 How It Works

1. The user enters student information.
2. The input values are converted into a Pandas DataFrame.
3. The trained SVM model predicts the placement status.
4. The prediction is displayed on the screen.

---

## 📷 User Interface

The application contains:

- Study Hours input
- Attendance input
- Sleep Hours input
- Internet Usage input
- Assignments Completed input
- Previous Score input
- Predict Placement button

---

## 📈 Future Improvements

- Display prediction probability
- Add data visualization
- Deploy on Streamlit Community Cloud
- Improve model accuracy with feature engineering
- Allow CSV file uploads for bulk predictions

---

## 👨‍💻 Author

Developed as a beginner Machine Learning project using Python and Streamlit to demonstrate classification model deployment.
