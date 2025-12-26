# Student Stress Prediction using the StudentLife Dataset

## 📌 Project Overview

This project is built on the **StudentLife dataset**, a large-scale, real-world behavioral dataset collected by **Dartmouth College (2013)** for academic research purposes. 

**Objective :** Predict student stress levels by analyzing daily behavioral patterns derived from smartphone sensor data, surveys, and self-reports.

The project emphasizes **real-world data handling**, including large-scale data ingestion, extensive preprocessing, feature engineering, exploratory data analysis, visualization, and predictive modeling.

---

## 📊 About the Dataset

The StudentLife dataset is a **multi-gigabyte, multi-modal, heterogeneous dataset** capturing real student life over an academic term.

### Dataset Characteristics

- **Participants:** 48 undergraduate and graduate students
- **Duration:** ~10 weeks (entire academic term)
- **Structure:** Distributed across multiple folders per participant and per modality
### Data Modalities

- **Real-time smartphone sensing data ( 2M+ entries )**
    
    - App usage 
    - Physical activity and motion
    - Conversation sensing
    - GPS and movement data
    - Phone lock/unlock events
        
- **EMA (Ecological Momentary Assessments)**
    
    - ~32,000 self-reported entries capturing stress, mood, sleep, and social interaction
        
- **Survey data**
    
    - Pre- and post-study psychological surveys
    - Stress, loneliness, sleep quality, personality traits

This diversity and scale make the dataset highly representative of **real-world, noisy, human-generated data**.

---

## 🛠️ Data Ingestion & Preprocessing

A major focus of this project was handling the **complexity of real-world data**:

- Ingested data from **multiple heterogeneous sources** spread across different directories
    
- Unified inconsistent schemas across modalities
    
- Aligned timestamps and aggregated high-frequency sensor logs into daily summaries
    
- Handled **missing and inconsistent data** caused by:
    
    - Irregular user participation
    - Inactive or unreliable sensors
    - Partial or skipped survey responses
        

Each preprocessing decision was carefully validated to preserve behavioral meaning while making the data suitable for analysis and modeling.

---

## ⚙️ Feature Engineering

Raw event-level data was transformed into **interpretable daily features**, where each row represents a student’s complete daily routine.

Examples include:

- Daily app usage intensity
- Sleep duration and sleep quality indicators
- Physical activity levels
- Social interaction frequency
- Survey-derived psychological metrics

Outliers and anomalies were identified through exploratory analysis to improve data quality and model robustness.

---

## 📈 Exploratory Data Analysis & Visualization

To extract insights and guide modeling decisions, extensive visualization was performed:

- **Univariate analysis** to understand feature distributions
- **Bivariate analysis** to explore relationships between behavioral factors and stress
- **Multivariate analysis** to study combined effects of lifestyle variables

Both **Seaborn** and **Plotly** were used to create interactive and static visualizations.

---

## 🤖 Modeling & Evaluation

The processed dataset was used to train classification models to predict whether a student is likely to experience stress.

- Binary and multi-class stress prediction
    
- Models evaluated using:
    
    - Precision
    - Recall
    - F1-score
        
- Addressed class imbalance and real-world label noise
    
The modeling stage focused not only on accuracy, but also on **behavioral interpretability**.

---

## 🎯 Key Takeaways

This project demonstrates the ability to:

- Handle **large-scale, messy, real-world datasets**
- Design robust preprocessing pipelines
- Perform meaningful exploratory analysis and visualization
- Engineer features from raw sensor data
- Build and evaluate predictive models on human behavioral data

Unlike clean benchmark datasets, this project reflects challenges commonly encountered in **production-level data science and machine learning workflows**.

---

## 🚀 Technologies Used

- Python
- Pandas, NumPy
- Seaborn, Plotly
- Scikit-learn
- PyTorch
    

---

## 📎 Acknowledgement

This project uses the **StudentLife dataset** collected by Dartmouth College for academic research purposes.