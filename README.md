# 📰 Fake News Detection System

A beginner-friendly **Machine Learning + Flask** project that classifies submitted news text as **FAKE NEWS** or **REAL NEWS**.

## Features

- 📰 News text input
- 🤖 TF-IDF text feature extraction
- 🧠 Logistic Regression classifier
- 📊 Prediction confidence
- 🌐 Flask web interface
- 📱 Responsive UI
- 📁 Local CSV training dataset
- 🔄 Automatic model training on first run

## Project Structure

```text
fake_news_detection_system/
│
├── app.py
├── train_model.py
├── requirements.txt
├── README.md
├── data/
│   └── news.csv
├── templates/
│   └── index.html
└── static/
    └── style.css
```

## How to Run in VS Code / PowerShell

### 1. Open the project folder

```powershell
cd path\to\fake_news_detection_system
```

### 2. Create a virtual environment

```powershell
python -m venv venv
```

### 3. Activate it

Windows PowerShell:

```powershell
.\venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, use:

```powershell
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
.\venv\Scripts\Activate.ps1
```

### 4. Install packages

```powershell
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 5. Train the model

```powershell
python train_model.py
```

You should see:

```text
Model trained successfully...
```

### 6. Start the website

```powershell
python app.py
```

Open the address shown by Flask, normally:

```text
http://127.0.0.1:5000
```

## Important

This project is suitable as an **educational ML demonstration**. The included dataset is intentionally small so that the project runs without downloading a large dataset. For a serious research project, replace `data/news.csv` with a much larger, properly labeled and sourced dataset and evaluate the model using train/test splits and metrics such as accuracy, precision, recall and F1-score.

The model detects linguistic patterns learned from its training data; it does **not independently verify whether a real-world claim is true**.

## Technologies

Python • Flask • Scikit-learn • TF-IDF • Logistic Regression • HTML • CSS • JavaScript
