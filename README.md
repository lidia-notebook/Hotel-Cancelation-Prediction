# Hotel Booking Demand Prediction

## Overview  
The hospitality industry has long focused on **occupancy rates** as a primary performance indicator. However, high occupancy does not necessarily guarantee profitability. Hotels face two major challenges:  

- **Cancellations** — rooms remain empty, resulting in lost revenue.  
- **Overbookings** — more guests arrive than available rooms, forcing costly relocations or free upgrades.  

This project aims to build a **predictive model** for booking cancellations and simulate **safe overbooking strategies**. By anticipating cancellations, hotels can optimize occupancy and profitability while maintaining customer satisfaction.  

---

## Objectives  
- Predict the likelihood of booking cancellations.  
- Identify key factors influencing cancellations.  
- Simulate overbooking strategies to minimize financial risk.  
- Provide actionable recommendations for hotel management.  

---

##  Workflow  

### 1. Business Understanding  
- Define the problem: cancellations vs. overbookings.  
- Establish metrics to balance recall (catching cancellations) and precision (avoiding false alarms).  

### 2. Data Preparation  
- Clean and preprocess the dataset: handle missing values, remove duplicates, and convert date features.  
- **Feature Engineering:**  
  - Lead time, length of stay, weekend vs. weekday.  
  - Average Daily Rate (ADR) per person.  
  - Historical cancellations, booking changes, and special requests.  
- Encode categorical variables: market segment, deposit type, customer type, reserved room type, country.  

### 3. Exploratory Data Analysis (EDA)  
- Analyze seasonal trends and booking patterns.  
- Explore correlations between features and cancellations.  
- Visualize cancellation rates by market segment, deposit type, and lead time.  

### 4. Modeling  
- Split dataset into training and testing sets.  
- Baseline model: **Logistic Regression**.  
- Advanced models: **Random Forest, XGBoost**.  
- Evaluation metrics: **Accuracy, Precision, Recall, F1-score, ROC-AUC**.  
- Focus on **Recall** to reduce the risk of underestimating cancellations.  

### 5. Simulation & Optimization  
- Estimate cancellation probabilities per booking.  
- Simulate safe overbooking strategies.  
- Provide guidelines for risk-aware overbooking policies.  

### 6. Evaluation & Insights  
- Assess financial and operational impact of predictions.  
- Translate model performance into business trade-offs:  

| Prediction Error | Impact on Business | Example Consequence |  
|------------------|--------------------|---------------------|  
| **False Negative** (predict “no cancel” but booking cancels) | Empty rooms, lost revenue | Unused inventory |  
| **False Positive** (predict “cancel” but booking arrives) | Overbooking risk | Guest relocation or upgrade |  

- Recommendations: targeted deposit policies, flexible upgrades, and segment-based strategies.  

---

## Tools & Technologies  
- **Programming Language:** Python  
- **Libraries:** pandas, NumPy, scikit-learn, XGBoost, Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook / Streamlit (for deployment prototype)  

---

## Business Impact  
- **Reduced Revenue Loss** → fewer empty rooms due to cancellations.  
- **Improved Guest Satisfaction** → minimize forced relocations.  
- **Optimized Occupancy** → balance between cancellations and overbookings.  

 

