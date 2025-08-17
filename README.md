# Deepfake Detection Website 🎭

A Django-based web application for detecting **deepfake videos** using a hybrid **CNN + LSTM** deep learning model.  
The system extracts frames from uploaded videos, processes them with a CNN to capture spatial features, and leverages an LSTM to model temporal dependencies for accurate detection.

---

## 🚀 Features
- Upload a video through a simple web interface.
- Preprocessing pipeline to extract frames from video.
- CNN extracts spatial (frame-level) features.
- LSTM models temporal sequence patterns.
- Returns **deepfake probability** and detection result.
- Django-powered website with clean UI.

---

## 🗂️ Project Structure
deepfake/
├── ml_app/ # Django app containing ML logic
│ ├── models/ # (Optional) trained model storage
│ ├── views.py # Video processing and detection pipeline
│ └── ...
├── templates/ # HTML templates for web UI
├── static/ # CSS, JS, images
├── db.sqlite3 # SQLite database (dev)
├── manage.py # Django project manager
├── requirements.txt # Python dependencies
└── README.md # Project documentation
