# **📌 Patient Waiting Time Analysis**  

## **📌 Overview**  
This project explores whether **patient demographics (age & sex) influence waiting times** in a healthcare setting. The study uses **real-world-inspired medical scheduling data** to analyze patterns and predict waiting times using **Machine Learning models**.  

The findings can help **optimize scheduling** and **improve healthcare efficiency** by identifying whether demographic factors impact patient wait times.  

---

## **📂 Dataset Overview**  

### **🔗 Data Source:**  
- Simulated medical office **appointment scheduling dataset**  
- **Timeframe:** January 1, 2015 – December 31, 2024  

### **📊 Key Data Fields:**  
- **Patient Demographics:** `age`, `sex`  
- **Appointment Details:** `appointment_date`, `appointment_time`, `appointment_status`  
- **Waiting Time:** `waiting_time` (target variable)  
- **Scheduling Trends:** `day_of_week`, `appointment_duration`  

---

## **🔧 How It Works**  

### **1️⃣ Data Preprocessing & Cleaning**  
- **Handled missing & noisy data** (dropped where appropriate).  
- **Converted DOB → Age** for easier analysis.  
- **Created age groups** to categorize patients.  
- **Standardized data** using `StandardScaler`.  

### **2️⃣ Exploratory Data Analysis (EDA)**  
- **Visualized waiting time trends** across age groups & sexes.  
- Used **box plots & clustered bar charts** to analyze patterns.  
- Identified **no strong correlations** between age/sex and wait time.  

### **3️⃣ Machine Learning Model Implementation**  
- Selected **Regression Analysis** as waiting time is a continuous variable.  
- **Tested multiple models**:  
  ✅ **Decision Tree Regressor**  
  ✅ **Random Forest Regressor**  
- **Feature Engineering:**  
  - **One-Hot Encoded** categorical data (`sex`, `day_of_week`).  
  - **Introduced Age-Sex Interaction** to check for demographic influence.  

---

## **🚀 Model Performance & Insights**  

| Model                         | MAE (Lower is better) | R² Score (Closer to 1 is better) |
| ----------------------------- | --------------------- | -------------------------------- |
| Decision Tree (max_depth=15)  | 0.7928                | -0.0572                          |
| Random Forest (max_depth=15)  | 0.7806                | -0.0145                          |

**Key Takeaways:**  
✅ **Age and sex do not significantly predict waiting time.**  
✅ **Negative R² scores indicate** demographic factors contribute little to wait times.  
✅ **Other factors (appointment type, clinic busyness) may be more relevant.**  

---

## **📈 Use Cases**  

- **Healthcare Scheduling Optimization** – Improve appointment efficiency.  
- **Patient Experience Analysis** – Identify factors influencing wait times.  
- **Operational Improvements** – Focus on non-demographic causes of delays.  

---

## **🛠 Tools Used**  

- **🐍 Python** – Data analysis & modeling  
- **📊 Pandas & NumPy** – Data manipulation  
- **📈 Matplotlib & Seaborn** – Visualization  
- **🤖 Scikit-Learn** – Machine Learning models  

---

## **🚀 Future Improvements**  

- **Include more features** (appointment type, clinic workload, time of day).  
- **Explore alternative models** (e.g., Gradient Boosting).  
- **Analyze time-series trends** in appointment delays.  

---

## **📞 Contact Information**  
📌 **Created by:** *Kyron Holbrook*  
📧 **Email:** *holbrookkyron@gmail.com*  
🔗 **Portfolio/GitHub:** [Sphynxalot](https://github.com/Sphynxalot)  
🔗 **LinkedIn:** [Kyron Holbrook](https://www.linkedin.com/in/kyron-holbrook/)  
