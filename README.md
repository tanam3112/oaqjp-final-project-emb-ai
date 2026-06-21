# Final Project - Emotion Detector

## Introduction

This repository contains the Final Project for the IBM Developing AI Applications with Python and Flask course.

The project implements an Emotion Detector application using the Watson NLP Emotion Prediction service. Users can submit text and receive emotion scores for:

* Anger
* Disgust
* Fear
* Joy
* Sadness

The application also identifies the dominant emotion in the submitted text.

## Features

* Emotion detection using Watson NLP
* Formatted JSON output
* Flask web deployment
* Error handling for invalid input
* Unit testing
* Static code analysis with pylint

## Project Structure

```text
EmotionDetection/
├── __init__.py
├── emotion_detection.py

templates/
├── index.html

server.py
test_emotion_detection.py
README.md
```

## Example Output

```python
{
    "anger": 0.01,
    "disgust": 0.00,
    "fear": 0.02,
    "joy": 0.92,
    "sadness": 0.01,
    "dominant_emotion": "joy"
}
```

## Running the Application

```bash
python server.py
```

Open the browser and visit:

```text
http://localhost:5000
```

## Testing

Run unit tests:

```bash
python test_emotion_detection.py
```

Run static code analysis:

```bash
pylint server.py
```

## Conclusion

This project demonstrates how Watson NLP services can be integrated into a Python Flask application to perform emotion analysis and return structured results to users.
