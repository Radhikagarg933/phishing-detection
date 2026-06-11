# 🛡️ PhishBoot – Phishing URL Detection System

PhishBoot is a Machine Learning-based web application that detects whether a given URL is **legitimate or phishing** using URL structure analysis and an XGBoost classification model. The project is built with **Python and Streamlit** for real-time predictions.

---

## 🚀 Features

* 🔗 Real-time phishing URL detection
* 🧠 Machine Learning model (XGBoost Classifier)
* ⚡ URL feature extraction using regex and parsing
* 💻 Interactive Streamlit web interface
* 📁 Model persistence using Joblib
* 🚨 Instant prediction (Phishing / Legitimate)

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Streamlit
* Joblib
* Regex (re)
* urllib.parse

---

## 📂 Project Structure

```id="phishboot1"
PhishBoot/
│
├── phishing_gui.py          # Streamlit application
├── phishing_model.pkl       # Trained ML model
├── phishing_dataset.csv     # Dataset used for training
└── README.md
```

---

## ⚙️ How It Works

1. User enters a URL in the Streamlit interface
2. System extracts features such as:

   * URL length
   * HTTPS usage
   * Number of dots
   * Presence of @ symbol
   * Presence of IP address
   * Hyphens in domain
3. Extracted features are passed to the ML model
4. XGBoost model predicts:

   * ✅ Legitimate URL
   * 🚨 Phishing URL
5. Result is displayed instantly

---

## ▶️ How to Run

### 1. Clone Repository

```bash id="phishboot2"
git clone https://github.com/Radhikagag933/phishing-detection.git
cd phishing-detection
```

---

### 2. Install Dependencies


```
pip install streamlit 
```

---

### 3. Run Application

```
streamlit run phishing_gui.py
```

---

### 4. Open in Browser

```text id="phishboot6"
http://localhost:8501
```

---

## 🧪 Sample Inputs

### Legitimate URL

```text id="phishboot7"
https://www.google.com
```

Output:

```text id="phishboot8"
✅ Legitimate Website
```

---

### Phishing URL

```text id="phishboot9"
http://secure-login-update-account.com
```

Output:

```text id="phishboot10"
🚨 Phishing Website Detected
```

---

## 📊 Model Details

* Algorithm: XGBoost Classifier
* Type: Binary Classification
* Output: Legitimate (0) / Phishing (1)
* Training: Based on URL feature dataset

---



## 🔮 Future Improvements

* Add WHOIS domain age check
* Integrate Google Safe Browsing API
* Improve feature engineering (keywords, subdomains)
* Add model comparison (Random Forest, Decision Tree)
* Improve accuracy with better dataset

---

#
