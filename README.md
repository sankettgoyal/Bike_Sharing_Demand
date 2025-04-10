# 🚲 Bike Sharing Demand Prediction

This project focuses on building a machine learning model to predict bike rental counts based on various temporal and environmental features. By analyzing both **daily** and **hourly** rental data, the model helps in forecasting future demand to optimize bike-sharing operations.

---

## 📁 Project Structure

```
├── artifacts/               # Stores trained models and evaluation outputs
├── documents/              # Contains project reports
│   └── Project Report/
├── logs/                   # Log files
├── notebook/               # Jupyter notebooks for exploration & modeling
│   └── data/               # Raw dataset files
├── src/                    # Source code
│   ├── components/         # Model and utility functions
│   └── pipeline/           # Training and preprocessing pipelines
├── static/                 # Static files for Flask app
├── templates/              # HTML templates for Flask app
```

---

## 📊 Dataset Overview

### `day.csv` — Daily Aggregated Data  
- `instant`: Unique record ID  
- `dteday`: Date  
- `season`: (1 = spring, 2 = summer, 3 = fall, 4 = winter)  
- `yr`: Year (0 = 2011, 1 = 2012)  
- `mnth`: Month (1–12)  
- `holiday`: Holiday flag (1 = Yes)  
- `weekday`: Day of the week (0 = Sunday)  
- `workingday`: Working day flag (1 = Yes)  
- `weathersit`: Weather condition (1–4 scale)  
- `temp`: Normalized temperature  
- `atemp`: Normalized "feels-like" temperature  
- `hum`: Normalized humidity  
- `windspeed`: Normalized windspeed  
- `casual`: Casual user count  
- `registered`: Registered user count  
- `cnt`: Total rentals  

### `hour.csv` — Hourly Data  
Includes all the fields from `day.csv`, plus:  
- `hr`: Hour of the day (0–23)

---

## ⚙️ Installation & Setup

### ✅ Prerequisites

- Python 3.7+
- `pip install -r requirements.txt`

### 🛠️ Steps to Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Pratik.94229/Bike-sharing-demand-prediction.git
   cd Bike-sharing-demand-prediction
   ```

2. **Create & Activate Virtual Environment (optional)**
   ```bash
   conda create -p venv python==3.8
   conda activate venv/
   ```

3. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

---

## 📈 Model Building & Evaluation

### Algorithms Used:
- Linear Regression  
- Random Forest  
- Extra Trees Regressor  
- LightGBM  
- XGBoost ✅ *(Best Performer)*

### Evaluation Metrics:
- Mean Absolute Error (MAE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

After extensive experimentation, **XGBoost** was chosen for deployment due to its high accuracy and robustness.

---

### 🧪 Run Locally with Flask

1. Train the model:
   ```bash
   python src/pipeline/training_pipeline.py
   ```

2. Launch Flask App:
   ```bash
   python app.py
   ```

3. Visit the local URL and enter inputs to get predictions.

---

## 📌 Results

The model successfully predicts bike-sharing demand using weather, calendar, and time-based features. The predictions can be used to improve fleet management, staff planning, and customer service.

---

## ✅ Conclusion

This project demonstrates how machine learning can effectively forecast real-world demand using environmental and temporal data. The interactive deployment with Streamlit and Flask ensures accessibility and ease of use for end users.
