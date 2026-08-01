# 🏙️ NYC Airbnb Room Type Predictor

<p align="center">

<img src="https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python">
<img src="https://img.shields.io/badge/FastAPI-0.115-green?style=for-the-badge&logo=fastapi">
<img src="https://img.shields.io/badge/Scikit--Learn-1.6-orange?style=for-the-badge&logo=scikitlearn">
<img src="https://img.shields.io/badge/Pandas-2.2-purple?style=for-the-badge&logo=pandas">
<img src="https://img.shields.io/badge/Deployed-Render-46E3B7?style=for-the-badge&logo=render">
<img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge">

</p>

---

# 🌐 Live Demo

### 🚀 https://nyc-airbnb-room-type-predictor-1-kdlh.onrender.com/

---

# 📖 Overview

NYC Airbnb Room Type Predictor is an end-to-end Machine Learning web application that predicts the most probable Airbnb room type from listing information.

The project combines:

- Machine Learning
- Data Preprocessing Pipeline
- FastAPI REST API
- Modern Responsive UI
- Production Deployment on Render

The application predicts one of the following room types:

- 🏠 Entire home/apt
- 🛏️ Private room
- 👥 Shared room

along with prediction probabilities.

---

# ✨ Features

✅ End-to-End ML Pipeline

✅ FastAPI Backend

✅ REST API

✅ Beautiful Dark UI

✅ Interactive Prediction Dashboard

✅ Probability Visualization

✅ Pydantic Validation

✅ Scikit-Learn Pipeline

✅ One-Hot Encoding

✅ Feature Scaling

✅ Production Deployment

---

# 📸 Screenshots

## Home Page

> Add screenshot here

```
images/home.png
```

---

## Prediction Result

> Add screenshot here

```
images/result.png
```

---

# 🎥 Demo

Add GIF here

```
images/demo.gif
```

(Record with ScreenToGif)

---

# 🏗 Project Architecture

```

                User

                  │

                  ▼

         HTML / CSS / JS

                  │

                  ▼

          FastAPI Backend

                  │

                  ▼

        Pydantic Validation

                  │

                  ▼

      Scikit-Learn Pipeline

        │
        ├── Missing Value Imputation
        ├── Feature Scaling
        ├── One-Hot Encoding
        └── Classification Model

                  │

                  ▼

         Predicted Room Type

                  │

                  ▼

        Probability Scores

```

---

# ⚙ Tech Stack

## Frontend

- HTML5
- CSS3
- JavaScript

---

## Backend

- FastAPI
- Pydantic

---

## Machine Learning

- Pandas
- NumPy
- Scikit-Learn
- Joblib

---

## Deployment

- Render

---

# 📂 Project Structure

```

NYC-Airbnb-Room-Type-Predictor/

│

├── main.py

├── Model_Pipeline.pkl

├── requirements.txt

├── runtime.txt

├── index.html

├── style.css

├── script.js

├── README.md

└── .gitignore

```

---

# 🧠 Machine Learning Workflow

```

Raw Dataset

↓

Data Cleaning

↓

Feature Selection

↓

Train Test Split

↓

Preprocessing Pipeline

↓

Model Training

↓

Evaluation

↓

Joblib Serialization

↓

FastAPI Deployment

↓

Prediction

```

---

# 🔄 Feature Engineering

The preprocessing pipeline automatically performs:

- Missing Value Imputation

- Standard Scaling

- One-Hot Encoding

- Column Transformation

- Feature Ordering

- End-to-End Pipeline Serialization

---

# 📊 Input Features

| Feature | Type |
|----------|------|
| Latitude | Float |
| Longitude | Float |
| Price | Float |
| Minimum Nights | Integer |
| Number of Reviews | Integer |
| Reviews per Month | Float |
| Host Listings Count | Integer |
| Availability 365 | Integer |
| Borough | Category |
| Neighbourhood | Category |

---

# 🎯 Prediction Classes

- Entire home/apt

- Private room

- Shared room

---

# 🌐 REST API

## GET /

Returns API status.

---

## POST /predict

### Sample Request

```json
{
"latitude":40.7128,
"longitude":-74.006,
"price":180,
"minimum_nights":2,
"number_of_reviews":15,
"reviews_per_month":1.4,
"calculated_host_listings_count":2,
"availability_365":320,
"neighbourhood_group":"Brooklyn",
"neighbourhood":"Williamsburg"
}
```

---

### Response

```json
{
"Predicted_room_type":"Entire home/apt",
"Probability":[
0.84,
0.12,
0.04
]
}
```

---

# 📈 Model Pipeline

```

Input

↓

Column Transformer

├── Numeric Pipeline

│ ├── Median Imputer

│ └── StandardScaler

│

└── Categorical Pipeline

├── Most Frequent Imputer

└── OneHotEncoder

↓

Classifier

↓

Prediction

```

---

# 🚀 Installation

Clone Repository

```bash
git clone https://github.com/AbhishekNimaje435/NYC-Airbnb-Room-Type-Predictor.git
```

Move into project

```bash
cd NYC-Airbnb-Room-Type-Predictor
```

Create Virtual Environment

```bash
python -m venv venv
```

Activate

Windows

```bash
venv\Scripts\activate
```

Install

```bash
pip install -r requirements.txt
```

Run

```bash
uvicorn main:app --reload
```

Open

```
http://127.0.0.1:8000
```

---

# 📊 Model Performance

| Metric | Value |
|----------|--------|
| Accuracy | XX % |
| Precision | XX % |
| Recall | XX % |
| F1 Score | XX % |

Replace with your actual values.

---

# 🚀 Future Improvements

- Docker

- CI/CD

- Kubernetes

- Authentication

- Database

- Model Monitoring

- Explainable AI

- SHAP Visualization

- Feature Importance

- User Login

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository

2. Create your branch

3. Commit changes

4. Push branch

5. Create Pull Request

---

# 📜 License

This project is licensed under the MIT License.

---

# 🙏 Acknowledgements

- NYC Airbnb Dataset

- Scikit-Learn

- FastAPI

- Pandas

- Render

---

# 👨‍💻 Author

## Abhishek Tikaramji Nimaje

Artificial Intelligence & Data Science Student

### GitHub

https://github.com/AbhishekNimaje435

---

# ⭐ Support

If you found this project useful,

please consider giving it a ⭐ on GitHub.

It helps others discover the project.
