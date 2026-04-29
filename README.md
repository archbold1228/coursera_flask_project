# Emotion Detector Web Application

## 📌 Project Overview

This project implements an **AI-based Emotion Detection Web Application** using the IBM Watson NLP library. The application analyzes user-provided text and identifies the dominant emotion along with confidence scores for multiple emotions.

The system is deployed as a web application using Flask and includes testing, error handling, and static code analysis.

---

## 🚀 Features

* Detects emotions from text input
* Returns scores for:

  * Anger 😠
  * Disgust 🤢
  * Fear 😨
  * Joy 😊
  * Sadness 😢
* Identifies the dominant emotion
* REST API using Flask
* Unit tested for reliability
* Error handling for invalid input
* Static code analysis compliant

---

## 🧠 Technologies Used

* Python 3.x
* IBM Watson NLP Library
* Flask (Web Framework)
* unittest (Testing)
* pylint (Static Code Analysis)

---

## 📂 Project Structure

```
EmotionDetection/
│
├── EmotionDetection/
│   ├── __init__.py
│   └── emotion_detection.py
│
├── test_emotion_detection.py
├── server.py
├── README.md
```

---

## ⚙️ Installation & Setup

1. Clone the repository:

```bash
git clone https://github.com/your-username/emotion-detector.git
cd emotion-detector
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Running the Application

Start the Flask server:

```bash
python server.py
```

Open your browser and navigate to:

```
http://localhost:5000
```

---

## 🧪 Running Unit Tests

```bash
python -m unittest test_emotion_detection.py
```

---

## 📊 Example Output

Input:

```
"I am very happy today!"
```

Output:

```json
{
  "anger": 0.01,
  "disgust": 0.02,
  "fear": 0.01,
  "joy": 0.94,
  "sadness": 0.02,
  "dominant_emotion": "joy"
}
```

---

## ⚠️ Error Handling

* Handles empty input
* Handles API errors (e.g., status code 400)
* Returns meaningful error messages

---

## 🧹 Static Code Analysis

Run pylint:

```bash
pylint server.py
```

Expected: **10/10 score**

---

## 📷 Screenshots

Screenshots for deployment and error handling are included as part of the project submission.

---

## 📌 Author

* Your Name

---

## 📄 License

This project is for educational purposes as part of an IBM AI Engineering course.

