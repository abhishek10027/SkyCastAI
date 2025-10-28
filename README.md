# SkyCastAI

SkyCastAI is an **AI-powered machine learning system** designed to predict the **weather type** based on environmental and atmospheric parameters. By leveraging multiple classification algorithms and structured data processing, this system provides accurate predictions, helping users understand and anticipate weather conditions effectively.

---

## **Objective**

Weather is influenced by factors such as **temperature, humidity, wind speed, precipitation, cloud cover, atmospheric pressure, UV index, season, visibility, and location**. SkyCastAI analyzes these factors to predict the **Weather Type** (Sunny, Cloudy, Rainy, Stormy), enabling users to plan activities and make informed decisions.

---
Perfect! Based on your variable descriptions and dataset shape, here’s a **clean Dataset Description section** you can directly include in your SkyCastAI README:

---

## **Dataset Description**

The dataset contains **historical weather data** collected from various locations, including inland, coastal, and mountainous regions. It consists of **13,200 observations** with **11 features**, including the target variable, **Weather Type**. The dataset captures a wide range of atmospheric and environmental conditions, including potential outliers in temperature, humidity, wind speed, precipitation, and visibility.

**Variables:**

| Variable             | Type        | Description                                                                 |
| -------------------- | ----------- | --------------------------------------------------------------------------- |
| Temperature          | Numeric     | Temperature in degrees Celsius, ranging from extreme cold to extreme heat.  |
| Humidity             | Numeric     | Humidity percentage, including values above 100% to introduce outliers.     |
| Wind Speed           | Numeric     | Wind speed in kilometers per hour, including unrealistically high values.   |
| Precipitation (%)    | Numeric     | Precipitation percentage, including outlier values.                         |
| Cloud Cover          | Categorical | Cloud cover description (e.g., clear, partly cloudy, overcast, cloudy).     |
| Atmospheric Pressure | Numeric     | Atmospheric pressure in hPa, covering a wide range.                         |
| UV Index             | Numeric     | Strength of ultraviolet radiation.                                          |
| Season               | Categorical | Season during which the data was recorded (Winter, Spring, Summer, Autumn). |
| Visibility (km)      | Numeric     | Visibility in kilometers, including very low or very high values.           |
| Location             | Categorical | Type of location where data was recorded (inland, coastal, mountain).       |
| Weather Type         | Categorical | Target variable for classification: Sunny, Cloudy, Rainy, or Stormy.        |

**Dataset Shape:** `(13200, 11)`

**Notes:**

* All categorical variables are encoded numerically for machine learning model compatibility.
* The dataset is suitable for **classification tasks** to predict weather type.
* Includes real-world and simulated outliers to test model robustness.

---

## **Features**

* **Multi-Model Evaluation:** Compares five classification algorithms to select the most reliable model.
* **Categorical Feature Encoding:** Converts non-numeric features into machine-readable formats for optimal model performance.
* **Performance Metrics:** Evaluates models using Accuracy, Precision, Recall, and F1-Score.
* **Interactive Prediction:** Allows users to enter weather parameters manually and receive instant predictions.
* **Scalable and Extensible:** Can incorporate additional features like air quality or geographic coordinates for improved prediction accuracy.

---

## **Data Preprocessing & Feature Encoding**

The system uses structured data with the following features:

**Numerical Features:**

* Temperature (°C)
* Humidity (%)
* Wind Speed (km/h)
* Precipitation (%)
* Atmospheric Pressure (hPa)
* UV Index
* Visibility (km)

**Categorical Features (Encoded Numerically):**

* Cloud Cover: clear → 1, partly cloudy → 2, overcast → 3, cloudy → 4
* Season: Winter → 1, Spring → 2, Summer → 3, Autumn → 4
* Location: inland → 1, coastal → 2, mountain → 3
* Weather Type (Target): Sunny → 1, Cloudy → 2, Rainy → 3, Stormy → 4

---

## **Model Evaluation**

The models were trained and evaluated on Accuracy, Precision, Recall, and F1-Score.

| Model               | Accuracy | Precision | Recall | F1-Score |
| ------------------- | -------- | --------- | ------ | -------- |
| Logistic Regression | 0.8705   | 0.8705    | 0.8705 | 0.8701   |
| Decision Tree       | 0.9117   | 0.9119    | 0.9117 | 0.9117   |
| Random Forest       | 0.9182   | 0.9185    | 0.9182 | 0.9182   |
| SVM                 | 0.8284   | 0.8332    | 0.8284 | 0.8278   |
| Gradient Boosting   | 0.9087   | 0.9090    | 0.9087 | 0.9086   |

**Best Model:** Random Forest

---

## **Confusion Matrix for Best Model**

The confusion matrix visually represents how well the best model (Random Forest) predicts each weather type. Correct predictions are along the diagonal, while misclassifications appear off-diagonal.

<img width="729" height="608" alt="image" src="https://github.com/user-attachments/assets/da2454f1-6596-4732-836d-f3a3d7c4ec77" />


---

## **Prediction Using User Input**

SkyCastAI allows users to **enter weather parameters manually** and get predictions in a readable format (Sunny, Cloudy, Rainy, Stormy).

**Workflow:**

1. **Input Data:** User provides values for temperature, humidity, wind speed, precipitation, cloud cover, pressure, UV index, season, visibility, and location.
    <img width="658" height="259" alt="image" src="https://github.com/user-attachments/assets/7e3d598b-a0c1-4a57-90cc-1e43e896dd5f" />

2. **Data Processing:** Categorical values are encoded into numeric format.
3. **Model Execution:** The pre-trained Random Forest model evaluates the expected weather type.
4. **Prediction Output:** Displays the predicted weather type.
   
   <img width="430" height="60" alt="image" src="https://github.com/user-attachments/assets/0d1f9682-f026-4991-8715-c4c157b0da09" />
   
---

## **Future Enhancements**

* Integrating **real-time weather API data** for live predictions.
* Incorporating **geospatial features** like altitude or proximity to water bodies.
* Adding ensemble techniques to combine multiple model predictions for improved accuracy.
* Developing a **web or mobile interface** for user-friendly interaction.

---

## **Conclusion**

SkyCastAI provides a **practical, interpretable, and reliable solution** for weather prediction. By analyzing key environmental features and leveraging machine learning, the system helps users anticipate weather conditions, enabling better planning and decision-making.

---

## **Developer**

**Abhishek Kushwaha**

🔗 LinkedIn: [https://www.linkedin.com/in/abhishek10027](https://www.linkedin.com/in/abhishek10027)

💻 GitHub: [https://github.com/abhishek10027](https://github.com/abhishek10027)


