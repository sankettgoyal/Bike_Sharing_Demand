# 🚲 Bike Sharing Demand Prediction

This project aims to develop a machine learning model to predict bike rental counts based on various temporal and environmental factors. By analyzing rental data, the model assists in forecasting demand, thereby optimizing bike-sharing operations.

---

## 📁 Project Structure

```
├── Bike Sharing Demand.py    # Main script for data processing and model training
├── README.md                 # Project documentation
├── requirements.txt          # List of required Python packages
```

---

## 📊 Dataset Overview

The dataset used in this project includes features such as:

- **Date**: Specific day of the rental
- **Season**: Categorical variable indicating the season (e.g., Spring, Summer)
- **Weather Situation**: Categorical variable describing weather conditions (e.g., Clear, Mist, Rain)
- **Temperature**: Normalized temperature in Celsius
- **Humidity**: Normalized humidity percentage
- **Windspeed**: Normalized wind speed
- **Casual Users**: Count of casual (non-registered) users
- **Registered Users**: Count of registered users
- **Total Count**: Total number of bike rentals (sum of casual and registered users)

---

## ⚙️ Installation & Setup

### ✅ Prerequisites

- Python 3.7 or higher

### 🛠️ Steps to Run Locally

1. **Clone the Repository**
   ```bash
   git clone https://github.com/sankettgoyal/Bike_Sharing_Demand.git
   cd Bike_Sharing_Demand
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Main Script**
   ```bash
   python "Bike Sharing Demand.py"
   ```

---

## 📈 Model Building & Evaluation

The project involves:

- **Data Preprocessing**: Handling missing values, encoding categorical variables, and feature scaling.
- **Model Training**: Implementing machine learning algorithms to predict bike rental counts.
- **Evaluation**: Assessing model performance using metrics such as Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R² Score.

---

## 📌 Results

The model provides insights into factors affecting bike rental demand and achieves satisfactory performance in predicting rental counts. These predictions can aid in decision-making for bike-sharing services, such as fleet management and resource allocation.

---

## ✅ Conclusion

This project demonstrates the application of machine learning techniques to forecast bike-sharing demand using temporal and environmental data. The insights gained can help optimize operations and improve user satisfaction in bike-sharing systems.
