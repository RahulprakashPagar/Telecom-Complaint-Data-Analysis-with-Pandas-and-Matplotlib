# Comcast Telecom-Consumer Complaints Analysis
A data analysis project that explores customer complaints received by Comcast, identifying major complaint types, trends, and state-wise resolutions using Python data analysis and visualization techniques.

# 📞 Comcast Telecom Consumer Complaints : Data Analytics Project

This project analyzes consumer complaints received by **Comcast**, a U.S. telecommunications company.  
The goal is to identify trends in complaint frequency, types, and resolution efficiency across states, helping to pinpoint key service issues and areas for improvement.

---

## 📊 Project Overview
- **Goal:** Analyze customer complaints and visualize complaint trends over time and across U.S. states.  
- **Dataset:** Comcast Telecom Complaints Dataset (CSV provided)  
- **Techniques Used:** Data Cleaning, Aggregation, Visualization, and Text Analysis  
- **Libraries:** pandas, matplotlib, numpy, seaborn  
- **Environment:** Jupyter Notebook (`P3.ipynb`) / Python 3.x  
- **Author:** [Rahul Pagar](https://www.linkedin.com/in/rahul-pagar1993)

---

### 🏷️ Keywords
data-analysis, python, pandas, matplotlib, seaborn, kaggle, telecom, consumer-complaints, data-visualization, machine-learning

---

## ⚙️ Workflow and Methods

### 1️⃣ Data Preparation
- Imported dataset using `read_csv()`  
- Verified structure, null values, and data types using `.info()` and `.describe()`  
- Combined date and time columns into a single datetime index for time-based analysis  
- Standardized date format and created trend visualizations  
- Prepared dataset for aggregation and analysis

### 2️⃣ Complaint Trend Analysis
- Extracted **month** and **year** from the date column to analyze complaint frequency.  
- Created **Daily** and **Monthly** trend charts to visualize patterns over time.  
- Found peak complaint activity during mid-2015, suggesting service disruptions.

### 3️⃣ Categorization of Complaint Status
- Simplified complaint status into two categories for better interpretation:  
  - **Open** → includes “Open” and “Pending”  
  - **Closed** → includes “Closed” and “Solved”  
- This helped measure the resolution ratio and compare closure efficiency across states.

### 4️⃣ Complaint Frequency and Type Analysis
- Grouped data to identify the most frequent complaint categories using `value_counts()` and `groupby()`.  
- Major themes: **Internet**, **Billing**, **Customer Service**, and **Network Issues**.  
- Computed topic percentages using simple keyword matching (e.g., “Internet”, “Billing”, “Customer Service”) to quantify category-level issues.

### 5️⃣ State-Wise Complaint Analysis
- Aggregated complaints by **State** and **Status (Open/Closed)**.  
- Identified states with the **maximum complaints** and **highest unresolved complaint ratios**.  
- Created stacked bar charts to visualize **Open vs Closed** complaint distribution by state.  
- Found that **California, Georgia, and Florida** had the highest number of complaints.

### 6️⃣ Insights and Key Findings
- The **majority of complaints** were related to **Internet** and **Billing** issues.  
- **Customer Service** concerns frequently appeared in textual complaints.  
- Complaint volume peaked during **June 2015**, indicating network or support issues during that period.  
- Roughly **20–25%** of all complaints remained unresolved, while others were marked as closed or solved.  
- Most complaints were received via **Internet submissions** and **Customer Care Calls**.

---

## 📈 Visualizations
- **Daily Complaint Trend** — visualizes day-to-day variations in complaint volume.  
- **Monthly Complaint Trend** — shows monthly complaint frequency trends.  
- **State-wise Open vs Closed Chart** — highlights resolution efficiency by state.  
- **Category Frequency Tables** — rank complaint topics by occurrence.  
- **Optional Pie Charts** — show proportions of complaint categories.

---

## 📑 Files, Author & Conclusion

### 📁 Files Included
- **`Comcast_telecom_complaints_data.csv`** — Original dataset used for analysis.  
- **`P3.ipynb`** — Jupyter Notebook containing the entire code, analysis, and visualizations.  
- **`Writeup for project (1).docx`** — Comprehensive project report detailing methodology and results.

### 👨‍💻 Author
**Rahul Pagar**    
🔗 [LinkedIn Profile](https://www.linkedin.com/in/rahul-pagar1993)

### 🏁 Conclusion
This analysis of the **Comcast Telecom Consumer Complaints Dataset** uncovers crucial insights about customer dissatisfaction and service performance.  
Key takeaways include:  
- **Internet** and **Billing** are the top areas of concern for customers.  
- **California, Georgia, and Florida** report the most complaints.  
- Around **75–80%** of complaints were resolved, while others remain open or pending.  
- Consolidating complaint statuses into **Open** and **Closed** categories enables a clearer understanding of service resolution efficiency.  

Overall, this project demonstrates how **Python’s pandas, matplotlib, and seaborn** libraries can be used for real-world telecom complaint analysis.  
Future improvements may include applying **sentiment analysis** on complaint text and building **predictive models** to forecast complaint resolution likelihood or customer churn risk.

---
