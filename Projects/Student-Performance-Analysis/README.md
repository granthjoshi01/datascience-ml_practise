# 📚 Student Performance Analysis

A beginner-friendly **Data Science and Machine Learning** project that analyzes student performance based on study hours, attendance, and exam scores. This project demonstrates fundamental concepts in data exploration, visualization, and predictive modeling.

---

## 🎯 Project Overview

This project explores the relationship between:
- **Study Hours**: Weekly study time
- **Attendance**: Percentage of classes attended
- **Exam Scores**: Final exam performance
- **Pass/Fail Status**: Binary classification (Pass = 1, Fail = 0)

### Key Objectives
1. Analyze patterns in student performance data
2. Visualize correlations between study habits and success
3. Build a machine learning model to predict pass/fail outcomes
4. Practice essential data science workflows

---

## 📊 Dataset

The project uses a **synthetic dataset** of 10 students with the following features:

| Feature | Description | Range |
|---------|-------------|-------|
| `Study_Hours` | Hours studied per week | 3-12 |
| `Attendance` | Class attendance percentage | 60-95% |
| `Exam_Score` | Final exam score | 50-92 |
| `Passed` | Pass/Fail status | 0 (Fail) or 1 (Pass) |

**Sample Data:**
```python
{
    "Name": ["Alice", "Bob", "Charlie", ...],
    "Study_Hours": [10, 5, 8, ...],
    "Attendance": [90, 70, 85, ...],
    "Exam_Score": [85, 55, 78, ...],
    "Passed": [1, 0, 1, ...]
}
```

---

## 🛠️ Technologies Used

- **Python 3.9+**
- **Libraries:**
  - `pandas` - Data manipulation
  - `numpy` - Numerical computing
  - `matplotlib` & `seaborn` - Data visualization
  - `scikit-learn` - Machine learning (Logistic Regression)

---

## 📈 Analysis & Visualizations

### 1. **Exploratory Data Analysis (EDA)**
- Summary statistics (mean, min, max)
- Average study hours for passers vs. failers
- Attendance patterns by performance

### 2. **Visualizations**

#### Scatter Plot: Study Hours vs Attendance
- Color-coded by Pass/Fail status
- Bubble size represents Exam Score
- Shows clear clustering: students with high study hours + attendance tend to pass

#### Box Plot: Exam Scores by Pass/Fail
- Compares score distributions
- Highlights median, quartiles, and outliers

---

## 🤖 Machine Learning Model

### Algorithm: **Logistic Regression**
- **Why?** Simple, interpretable, effective for binary classification
- **Features:** Study_Hours, Attendance, Exam_Score
- **Target:** Passed (0/1)

### Model Pipeline
1. **Feature Scaling** using `StandardScaler` (normalizes data)
2. **Train-Test Split** (70-30)
3. **Cross-Validation** (5-fold) for robust evaluation
4. **Prediction** on new student data

### Performance Metrics
```
Model Accuracy: ~70-100% (varies by random split)
Cross-Validation Accuracy: 1.0 ± 0.0
```

**Note:** With only 10 samples, accuracy is high but may not generalize to larger datasets. This is a learning exercise!

---

## 🚀 How to Run

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Steps
1. **Clone the repository** (or download the notebook)
   ```bash
   git clone <your-repo-url>
   cd student-performance-analysis
   ```

2. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

3. **Open the notebook** (`student_performance_analysis.ipynb`)

4. **Run all cells** (Cell → Run All)

5. **Explore the results:**
   - View summary statistics
   - Analyze visualizations
   - Check model predictions

---



## 🔍 Key Insights

### Findings
1. **Study Hours Matter**: Students studying 9+ hours/week have a 100% pass rate
2. **Attendance Correlation**: 86% average attendance for passers vs. 65% for failers
3. **Combined Effect**: High study time + attendance = strong predictor of success

### Model Prediction Example
```python
New Student: 8 hours/week, 85% attendance, 78 exam score
Prediction: PASS ✅
```

---

## 🎓 Learning Outcomes

By completing this project, you'll learn:
- ✅ Data cleaning and preprocessing
- ✅ Statistical summary and grouping
- ✅ Creating informative visualizations (scatter plots, box plots)
- ✅ Training a machine learning classifier
- ✅ Evaluating model performance (accuracy, classification report)
- ✅ Cross-validation techniques
- ✅ Making predictions on new data

---

## 🔮 Next Steps & Improvements

### For Beginners
1. **Use a Real Dataset**: Download from [Kaggle](https://www.kaggle.com/datasets) (e.g., "Student Performance Dataset")
2. **Add More Features**: Include gender, parental education, etc.
3. **Try Other Models**: Decision Trees, Random Forests, SVM


---



**Happy Learning! 🎉**


