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
<img width="551" height="398" alt="Screenshot 2025-08-17 090854" src="https://github.com/user-attachments/assets/c65aa09e-e663-4f2c-b5f1-739d12a28b24" />


---

## ⚙️ Installation & Setup

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Vikaskoppoju/deepfake.git
cd deepfake
```
### 2️⃣ Create a virtual environment
```bash
python -m venv .venv
source .venv/bin/activate   # On Linux/Mac
.venv\Scripts\activate      # On Windows
```
### 3️⃣ Install dependencies
```bash
pip install -r requirements.txt
```
### 4️⃣ Apply migrations
```bash
python manage.py migrate
```
### 6️⃣ Run the development server
```bash
python manage.py runserver
```
Now visit 👉 http://127.0.0.1:8000/ in your browser.

## 🧠 Model Details

- CNN extracts spatial features from individual frames.

- LSTM learns temporal dependencies across frame sequences.

- Model trained on deepfake video datasets (e.g., FaceForensics++ or DFDC).

- Outputs probability score and class label (Real / Fake).

### 📌 Usage

- Open the website in your browser.

- Upload a video file (.mp4, .avi, etc.).

- The system will:

-- Extract frames

-- Pass through CNN + LSTM model

- Return whether the video is Deepfake or Authentic.

- Results displayed on the UI.



















