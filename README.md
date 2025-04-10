# 🚲 Bike Sharing Demand Prediction

This project focuses on building a machine learning model to forecast bike rental demand based on various features like date, weather conditions, and time. It uses historical bike-sharing data to help optimize resource planning for such services.

---

## 📦 Installation

You can install the dependencies directly using the `setup.py` script:

```bash
git clone https://github.com/sankettgoyal/Bike_Sharing_Demand.git
cd Bike_Sharing_Demand
pip install .
```

Alternatively, use the traditional method:

```bash
pip install -r requirements.txt
```

---

## 📁 Project Structure

```
├── Bike Sharing Demand.py     # Main notebook/script for training and evaluation
├── requirements.txt           # Required packages
├── setup.py                   # Project installation script
├── README.md                  # Project documentation
```

---

## 📊 Dataset Description

The dataset includes both **daily** and **hourly** bike rental records with the following features:

- `season`, `yr`, `mnth`, `hr`, `holiday`, `weekday`, `workingday`
- Weather: `weathersit`, `temp`, `atemp`, `hum`, `windspeed`
- Target columns: `casual`, `registered`, `cnt` (total count of rentals)

---

## 🧠 Model Development

The following machine learning models were tested:

- Linear Regression  
- Random Forest  
- Extra Trees Regressor  
- LightGBM  
- XGBoost ✅ *(Best performing model)*

### ✅ Final Model:
**XGBoost** was chosen for its superior performance across evaluation metrics like MAE, RMSE, and R².

---

## ⚙️ How to Run

After installation, you can run the training and prediction pipeline with:

```bash
python "Bike Sharing Demand.py"
```

---

## 📈 Results

The model effectively predicts bike rental counts and provides actionable insights for operational planning. Predictions were evaluated using:

- 📉 Mean Absolute Error (MAE)
- 📉 Root Mean Squared Error (RMSE)
- 📈 R² Score

---

## ✅ Conclusion

This project showcases the power of machine learning for solving real-world forecasting problems. With proper preprocessing and model tuning, we achieved a reliable demand prediction system for bike sharing.

---

## 🛠️ Technologies Used

**Languages & Tools:** Python, Jupyter Notebook  
**Libraries:** NumPy, Pandas, Matplotlib, Scikit-learn, XGBoost, LightGBM  
**Utilities:** pip, setuptools, VS Code, Git
