# Emotion Detection Web Application

A web-based Natural Language Processing (NLP) application that analyzes user-provided text and detects the dominant emotion using IBM Watson's Emotion Analysis service.

The application combines a Flask backend, a simple HTML/JavaScript frontend, and an external NLP API to classify emotions such as joy, sadness, anger, fear, and disgust.

---

## Project Overview

This project demonstrates the integration of a web application with a cloud-based NLP service for real-time emotion detection.

Users can enter any English sentence into the web interface, and the application returns:

- Anger score
- Disgust score
- Fear score
- Joy score
- Sadness score
- Dominant emotion

The backend communicates with IBM Watson's Emotion Detection API, processes the response, and sends the results back to the browser.

---

## Features

- Analyze emotions from user-provided text
- Detect the dominant emotion
- Display individual emotion confidence scores
- Interactive web interface
- REST API endpoint using Flask
- Unit tests for emotion classification

---

## Technologies Used

- Python
- Flask
- HTML5
- JavaScript
- IBM Watson NLP API
- Requests
- Unit Testing (unittest)

---

## Repository Structure

```text
Emotion-Detection-Web-App/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── app/
│   ├── server.py
│   │
│   ├── EmotionDetection/
│   │   ├── __init__.py
│   │   └── emotion_detection.py
│   │
│   ├── templates/
│   │   └── index.html
│   │
│   └── static/
│       └── mywebscript.js
│
└── tests/
    └── test_emotion_detection.py
```

---

## Installation

Clone the repository

```bash
git clone https://github.com/yourusername/Emotion-Detection-Web-App.git
cd Emotion-Detection-Web-App
```

Create a virtual environment

```bash
python -m venv venv
```

Activate the virtual environment

### Windows

```bash
venv\Scripts\activate
```

### macOS / Linux

```bash
source venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

## Running the Application

Start the Flask server

```bash
python app/server.py
```

Open your browser and navigate to

```text
http://localhost:5000
```

Enter a sentence into the text box and click **Run Sentiment Analysis** to view the detected emotions.

---

## Running Unit Tests

Run the test suite using

```bash
python -m unittest tests/test_emotion_detection.py
```

The tests verify that the emotion detector correctly identifies the dominant emotion for several example sentences.

---

## Example Input

```text
I am extremely happy today!
```

Example Output

```text
Anger: 0.01

Disgust: 0.00

Fear: 0.02

Joy: 0.96

Sadness: 0.01

Dominant Emotion: Joy
```

---

## Skills Demonstrated

- Natural Language Processing
- REST API Integration
- Flask Web Development
- Python Programming
- Frontend and Backend Communication
- JSON Processing
- Unit Testing
- API Requests
- Web Application Development

---

## Future Improvements

Potential enhancements include:

- Display results using charts or progress bars
- Add emotion history
- Support multiple languages
- Improve frontend styling
- Deploy the application to Render or Railway
- Containerize the application using Docker

---

## Author

Samantha Aranibar

