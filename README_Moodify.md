# 🎧 Moodify: An Emotion-Based Music Recommender

Moodify is a real-time emotion-based music recommendation system that uses facial expression analysis to recommend songs that match the user's current emotional state. By leveraging a Convolutional Neural Network (CNN) trained on the FER2013 dataset and integrating with the Spotify API, Moodify personalizes music experiences dynamically as your emotions change.

---

## 🎯 Project Highlights

- 🎥 Real-time facial emotion detection using webcam feed
- 🧠 Deep Learning model (CNN) trained on the FER2013 dataset
- 🎵 Spotify API integration for emotion-aligned music recommendations
- 🌐 Flask web app with live video stream and dynamic song suggestions
- 📊 Detailed evaluation with accuracy, confusion matrix, ROC curve, and more

---

## 📸 Demo

![Moodify UI](https://your-link-to-demo-screenshot.com)  
_Live detection and instant playlist recommendations._

---

## 🛠 Technologies Used

| Technology     | Purpose                           |
|----------------|------------------------------------|
| Python         | Core programming language         |
| TensorFlow/Keras | Deep learning model for emotion classification |
| OpenCV         | Real-time face detection and image preprocessing |
| Spotipy        | Python client for Spotify Web API |
| Flask          | Web application framework         |
| Pandas, NumPy  | Data processing and handling       |
| Matplotlib     | Data visualization and evaluation metrics |

---

## 📂 Project Structure

```
Moodify/
├── app.py                   # Main Flask app
├── camera.py                # Handles video capture and emotion detection
├── train.py                 # Model training script
├── Spotipy.py               # Spotify playlist fetch script
├── emotion_detection_model.keras  # Trained model file
├── songs/                   # Emotion-wise CSV playlists
├── templates/               # HTML files (index.html)
├── static/                  # CSS and JS assets
├── haarcascade_frontalface_default.xml  # Face detection XML
├── utils.py                 # Supporting utility functions
```

---

## 📊 Dataset Used

- **FER2013**: Facial Expression Recognition 2013
  - **Images**: 35,887 grayscale images (48x48)
  - **Classes**: Angry, Disgust, Fear, Happy, Neutral, Sad, Surprise
  - **Split**: 28,709 for training, 7,178 for testing

---

## 🚀 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/TheDevilPython/Moodify.git
cd Moodify
```

### 2. Create Virtual Environment
```bash
python -m venv moodify-env
source moodify-env/bin/activate  # or moodify-env\Scripts\activate on Windows
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Set Environment Variables
Add your Spotify credentials:
```bash
set SPOTIPY_CLIENT_ID=your_client_id
set SPOTIPY_CLIENT_SECRET=your_client_secret
```

### 5. Run the App
```bash
python app.py
```

---

## 📈 Model Training (Optional)

To retrain the model:

```bash
python train.py
```

It includes:
- Data augmentation
- Accuracy/loss visualization
- Early stopping
- Evaluation metrics like confusion matrix, ROC curve

---

## 📑 Key Features

- Real-time facial expression capture
- CNN-based emotion classification
- Spotify API integration using Spotipy
- Dynamic web UI to show current mood and playlist
- Downloadable CSVs of songs for each mood
- Fully modular and extensible

---

## 📷 Screenshots

| Live Emotion Detection | Song Recommendations |
|------------------------|----------------------|
| ![cam](https://your-link.com/cam.png) | ![songs](https://your-link.com/songs.png) |

---

## 📌 Future Improvements

- Add support for multi-modal emotion detection (voice + text)
- Improve playlist personalization based on past emotion history
- Add speech-based interaction
- Deploy via Docker or on cloud (Heroku, AWS)

---

## 📄 License

This project is licensed under the MIT License. Feel free to use and modify.

---

## 👨‍💻 Author

Made with ❤️ by [Your Name]  
GitHub: [TheDevilPython](https://github.com/TheDevilPython)