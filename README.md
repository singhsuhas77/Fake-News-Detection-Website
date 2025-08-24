# 📰 Fake News Detection Website

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)

This project is a web-based application designed to detect and classify fake news articles using Natural Language Processing (NLP) and Machine Learning. Users can paste the text of a news article into the interface, and the system will predict whether the news is REAL or FAKE based on a pre-trained model.

---

## ✨ Key Features

* **Accurate Prediction**: Utilizes a trained **Passive Aggressive Classifier** model to achieve high accuracy in detecting fake news.
* **Simple Web Interface**: A clean and user-friendly interface built with **Flask** that allows for easy text input and clear presentation of the prediction results.
* **NLP Pipeline**: Implements a robust text processing pipeline including stopword removal and TF-IDF vectorization to analyze news content effectively.
* **Scalable Backend**: Built with a lightweight and efficient Flask server. 

---

## ⚙️ How It Works

The detection process follows a standard machine learning pipeline for text classification:

1.  **Text Input**: The user provides the text of a news article through the web form.
2.  **Preprocessing**: The input text is cleaned and preprocessed. This involves removing stopwords (common words like "the", "is", "in") to focus on meaningful content.
3.  **Feature Extraction**: The preprocessed text is transformed into a numerical representation using a **TF-IDF (Term Frequency-Inverse Document Frequency) Vectorizer**. This technique highlights words that are important to the context of the article.
4.  **Prediction**: The resulting TF-IDF vector is fed into the pre-trained **Passive Aggressive Classifier model**, which outputs a prediction: "REAL" or "FAKE".

---

## 🛠️ Technology Stack

* **Backend**: Python, Flask
* **Machine Learning**: Scikit-learn, Pandas, NumPy
* **NLP**: NLTK (for stopwords)
* **Frontend**: HTML, CSS

---

## 🚀 Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

* Python 3.x installed on your machine.
* Pip for installing Python packages.

### Installation & Setup

1.  **Clone the Repository**
    ```bash
    git clone [https://github.com/singhsuhas77/Fake-News-Detection-Website.git](https://github.com/singhsuhas77/Fake-News-Detection-Website.git)
    cd Fake-News-Detection-Website
    ```

2.  **Create a Virtual Environment (Recommended)**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install Dependencies**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Application**
    ```bash
    python app.py
    ```

5.  Open your web browser and navigate to `http://127.0.0.1:5000` to use the application.

---

## 📊 Dataset

The model was trained on a dataset containing thousands of real and fake news articles. The dataset (`train.csv`) includes columns for the news text and a label indicating its authenticity.

---

## 🤝 Contributing

Contributions are welcome! If you have ideas for improvements or find any issues, feel free to open an issue or submit a pull request.

1.  Fork the Project
2.  Create your Feature Branch (`git checkout -b feature/NewFeature`)
3.  Commit your Changes (`git commit -m 'Add some NewFeature'`)
4.  Push to the Branch (`git push origin feature/NewFeature`)
5.  Open a Pull Request
