# Deep_Learnin_Project


## 1. Introduction  
In this project, we worked as a group team of two. My friend Emrah Fidan and I collaborated to complete this project together.  

Denial of Service (DoS) attacks remain one of the most significant threats to web services and network infrastructure. This project explores various machine learning and deep learning approaches to detect and classify DoS attacks, leveraging both traditional classification algorithms and advanced neural network architectures.  

## 2. Data Preprocessing and Feature Engineering  

### 2.1 Exploratory Data Analysis (EDA)  
- **Dataset structure:** Examined for missing values, duplicates, and basic statistics.  
- **Visualization:** Flow duration histograms, target variable distribution, and categorical feature analysis.  

### 2.2 Feature Engineering  
- **Packet Rate Calculation:** Packets per second derived.  
- **Protocol Frequency Analysis:** Normalized protocol occurrence rates.  
- **Data Quality Management:** Handling of NaN and infinite values.  

### 2.3 Feature Selection  
- **Correlation-Based Selection:** Top 50 features selected based on correlation with the target variable.  
- **Mutual Information Selection:** Importance scores computed for feature ranking.  

## 3. Traditional Machine Learning Approaches  
The following models were evaluated for detecting DoS attacks:  
- **Logistic Regression**  
- **Random Forest**  
- **XGBoost**  
- **LightGBM**  

## 4. Deep Learning Approaches  
To improve detection, deep learning models were implemented:  
- **Recurrent Neural Networks (RNN)**  
- **Long Short-Term Memory (LSTM)**  
- **Gated Recurrent Unit (GRU)**  

### 4.1 Complex Neural Network Architecture  
A hybrid ensemble model combining **CNN, LSTM, BiLSTM, and GRU** was developed for enhanced performance.  

## 5. Results and Comparisons  
All models performed exceptionally well in detecting HTTP-based DoS attacks.  

| Model               | Accuracy | Precision | Recall  | F1-Score | AUC    |  
|---------------------|----------|------------|--------|----------|--------|  
| Logistic Regression | 0.9996   | 0.9970     | 0.9911 | 0.9941   | 1.0000 |  
| Random Forest      | 1.0000   | 1.0000     | 1.0000 | 1.0000   | 1.0000 |  
| XGBoost           | 1.0000   | 1.0000     | 1.0000 | 1.0000   | 1.0000 |  
| LightGBM          | 1.0000   | 1.0000     | 1.0000 | 1.0000   | 1.0000 |  
| RNN               | 0.9998   | 0.9942     | 1.0000 | 0.9971   | 1.0000 |  
| LSTM              | 0.9999   | 1.0000     | 0.9971 | 0.9985   | 1.0000 |  
| GRU               | 0.9999   | 1.0000     | 0.9971 | 0.9985   | 1.0000 |  
| Ensemble          | 0.9999   | 1.0000     | 0.9970 | 0.9985   | 1.0000 |  

### 5.1 Key Findings  
- **Traditional ML models (RF, XGBoost, LightGBM) achieved perfect detection rates with lower computational cost.**  
- **Deep learning models (LSTM, GRU) performed similarly well, making them viable for real-time detection.**  

For full details, refer to the complete project report.  
