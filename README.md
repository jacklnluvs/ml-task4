# 🤖 AI-Powered Customer Feedback Classification System

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python)
![Machine Learning](https://img.shields.io/badge/ML-Naive%20Bayes-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Project Overview

This project is an **AI & Machine Learning-based system** that automatically classifies customer feedback into predefined categories and routes it to the appropriate department.

It uses **Natural Language Processing (NLP)** techniques and a **Naive Bayes classifier** to analyze text data and predict the category of feedback.

---

## 🚀 Features

* 🔍 Automatic classification of customer feedback
* 📊 Data visualization using bar charts
* ☁️ Word cloud generation for text insights
* ⚡ Real-time user input prediction
* 📌 Department routing system

---

## 🧠 How It Works

1. Load customer feedback dataset
2. Preprocess text data
3. Convert text into numerical format using CountVectorizer
4. Train model using Multinomial Naive Bayes
5. Predict category for new feedback
6. Route to respective department

---

## 🏗️ Project Architecture

---

## 🛠️ Technologies Used

* **Python**
* **Pandas**
* **Scikit-learn**
* **Matplotlib**
* **WordCloud**

---

## 📂 Dataset

The dataset used:

* `customer_feedback.csv`

### Columns:

* `Feedback` → Customer message
* `Category` → Label (Billing, Delivery, Product, etc.)

---

## ⚙️ Model Implementation

The model is built using a pipeline:

```python
Pipeline([
    ("vectorizer", CountVectorizer()),
    ("classifier", MultinomialNB())
])
```

This combines:

* Text vectorization
* Classification model

---

## 📊 Output Visualizations

### 1. Category Distribution
<img width="728" height="438" alt="Screenshot 2026-08-02 123020" src="https://github.com/user-attachments/assets/a2f334e4-ab48-4c99-bf36-7b0bffc28e7d" />

### 2. Word Cloud
<img width="915" height="434" alt="Screenshot 2026-08-02 122955" src="https://github.com/user-attachments/assets/025745e8-e2d2-4b53-87f1-ab3f7173e2a0" />

---

## 🔄 Feedback Routing System

After prediction, feedback is routed automatically:

| Category          | Department             |
| ----------------- | ---------------------- |
| Billing           | Finance Team           |
| Delivery          | Logistics Team         |
| Product           | Quality Assurance Team |
| Technical Support | IT Support Team        |
| General Inquiry   | Customer Care Team     |

---

## 🧪 Example

**Input:**

```
The payment failed and I was charged twice
```

**Output:**

```
Predicted Category: Billing
Route To: Finance Team
```

---

## ▶️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2. Install dependencies:

```bash
pip install pandas scikit-learn matplotlib wordcloud
```

3. Run the script:

```bash
python your_script.py
```

---

## 📈 Model Performance

* Accuracy is calculated using:

```python
accuracy_score(y_test, y_pred)
```

* Achieves good performance for basic text classification tasks.

---

## 🎯 Applications

* Customer support automation
* Helpdesk ticket routing
* Complaint management systems
* E-commerce feedback analysis

---

## 📌 Future Improvements

* Use advanced NLP models (BERT, Transformers)
* Add GUI or Web Interface
* Improve dataset size and quality
* Deploy as API or web app

---

## 👩‍💻 Author

**Jacklyne A**
BCA Student | Aspiring AI & Full Stack Developer

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!

---
