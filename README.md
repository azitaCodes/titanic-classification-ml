# 🚢 Titanic Survival Prediction (Beginner ML Project)

This project uses machine learning to predict if a passenger survived the Titanic disaster. It covers everything from cleaning the data to building and evaluating models.

Everything is written in a simple way, so even if you're new to ML, you can understand it easily.

---

## 📚 What This Project Covers

- Cleaned real-world data (Titanic dataset)
- Created new features like FamilySize
- Used Logistic Regression and Random Forest models
- Compared the models using accuracy and AUC
- Visualized results with confusion matrix and ROC curve

---

## 📊 Goal

The goal is to predict who survived based on information like:

- Age  
- Sex  
- Ticket class (Pclass)  
- Fare  
- Number of family members  
- Where they boarded (Embarked)

---

## 📁 Dataset Used

This is a public Titanic dataset from Kaggle. You can also download it from here:

```
https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv
```

---

## 🔧 Steps Followed

### 1. Load and Explore the Data
Checked the data structure, missing values, and distributions.

### 2. Data Cleaning
- Filled missing Age using median based on Pclass and Sex
- Filled Embarked with the most frequent value
- Removed extreme Fare outliers (capped at 99th percentile)
- Dropped irrelevant columns like Cabin, Ticket, and Name

### 3. Feature Engineering
- Created `FamilySize = SibSp + Parch`
- Encoded Sex and Embarked as numeric

### 4. Modeling
- Trained two models: Logistic Regression and Random Forest
- Split the data into train (80%) and test (20%)

### 5. Evaluation
- Metrics used:
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion matrix
  - ROC curve and AUC score

---

## ✅ Model Results

| Model               | Accuracy | AUC Score |
|---------------------|----------|-----------|
| Logistic Regression | 82%      | 0.89      |
| Random Forest       | 83%      | 0.90      |

---

## 📷 Visual Results

### ROC Curve  
![ROC Curve](images/roc_curve.png)

### Confusion Matrices  
**Logistic Regression**  
![Log Confusion](images/confusion_log.png)

**Random Forest**  
![RF Confusion](images/confusion_rf.png)

---

## 💡 Key Learnings

- How to work with real, messy data
- How to apply data cleaning techniques
- How to use basic classification models
- How to evaluate models using proper metrics
- How to create visualizations to explain results

---

## 🛠 How to Run It

### 1. Install needed libraries

Use the `requirements.txt` file:
```bash
pip install -r requirements.txt
```

Or manually install:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 2. Run the Notebook

Open `titanic_classification.ipynb` in Jupyter Notebook or VS Code and run each cell.

---

## 🙋‍♀️ About the Author

Azita Ramezani  
PhD Student | Machine Learning in Healthcare  
🔗 [LinkedIn](https://www.linkedin.com/in/azita-ramezani-722117275/) 

---

Thanks for visiting this project! ⭐
