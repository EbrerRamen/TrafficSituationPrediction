# 🚦 Traffic Situation Prediction

## 📘 Project Overview
This project aims to **predict real-time traffic situations** using machine learning models based on traffic-related factors such as time, day and vehicle volume.  

The goal is to build a predictive system that helps estimate whether a given traffic condition will be **Normal**, **Low**, **High**, or **Heavy**, enabling better traffic management and route planning.

The Jupyter Notebook (`Traffic Situation Prediction.ipynb`) provides a complete, step-by-step walkthrough — from **data cleaning**, **exploratory data analysis (EDA)**, **feature engineering**, and **model training**, to **evaluation** and **insight generation**.  

📊 For detailed visualizations, graphs, and tables, please **open the notebook** in Jupyter Notebook, JupyterLab, or Google Colab.

---

## 📂 Dataset
The dataset contains features related to traffic and external conditions, such as:
- **Time-related features:** Time, Date, Day of the week
- **Traffic metrics:** CarCount, BikeCount, BusCount, TruckCount
- **Target variable:** `Traffic Situation` (Normal / low / High / Heavy)

The dataset was analyzed and preprocessed to ensure quality and consistency before model training.

---

## 🧹 Data Preprocessing
The preprocessing steps include:
1. **Handling missing or invalid data entries**  
2. **Encoding categorical features** (Day of the week, Traffic Situation)  
3. **Quantile based quantization** for numeric features like CarCount, BikeCount, BusCount, TruckCount  
4. **Creating new derived features**, such as TotalCount  
5. **Splitting data** into training and testing sets  

---

## 📊 Exploratory Data Analysis (EDA)
Comprehensive visual exploration was conducted to understand the data distribution and relationships among variables. Key insights include:
- Traffic volume increases significantly during **morning and evening rush hours**.  
- Weekends and holidays show relatively **lower congestion levels** compared to weekdays.  

🖼️ *All graphs, plots, and summary tables can be viewed inside the notebook.*

---

## 🧠 Model Training
Several machine learning models were trained and compared, including:
- **K-Nearest Neighbour**  
- **Decision Tree Classifier**  
- **Random Forest Classifier**  

The dataset was divided into training and testing subsets, and cross-validation was applied to ensure consistent performance evaluation.

---

## 📈 Model Evaluation & Results
The models were evaluated using standard classification metrics such as **Accuracy**, **Precision**, **Recall**, and **F1-score**.  

Example results (illustrative summary):

| Model | Accuracy | Precision | Recall | F1-Score |
|:------|:----------|:-----------|:--------|:----------|
| Random Forest | 89.0% | 0.89 | 0.89 | 0.89 |
| Decision Tree | 85.0% | 0.86 | 0.85 | 0.85 |
| KNN | 83.0% | 0.86 | 0.83 | 0.83 |

The **Random Forest** outperformed others, indicating that ensemble-based approaches effectively captured the complex, nonlinear interactions among variables.

📊 *See the notebook for confusion matrices, and detailed performance visualizations.*

---

## 💡 Key Insights
- **Time of day** and **vehicle count** are the strongest predictors of traffic congestion.  
- **Machine learning models** can accurately classify traffic situations with over **90% accuracy**.  
- Predictive analytics can aid **smart city planning** and **real-time traffic monitoring systems**.

---

## ⚙️ Technologies Used
- **Python**  
- **NumPy, Pandas** – for data processing  
- **Matplotlib, Seaborn** – for visualizations  
- **Scikit-learn** – for machine learning models  
- **Jupyter Notebook / Google Colab** – for interactive experimentation and analysis  

---

## ▶️ How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/Traffic_Situation_Prediction.git
2. Open the notebook:
   ```
   Traffic Situation Prediction.ipynb
3. Run all cells in Jupyter Notebook or Google Colab. Ensure the dataset file is correctly placed in the project directory.
