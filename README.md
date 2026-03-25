🪞 Smart Mirror AI

A smart mirror built with Python and computer vision that detects facial expressions in real time and adapts its interface accordingly.
The project runs on a Raspberry Pi with a camera module and provides an interactive dashboard with emotion-aware features.

 Features
            Real-time Emotion Detection
            Uses a Convolutional Neural Network (CNN) to classify 7 emotions:
            happy, sad, angry, surprise, fear, disgust, neutral
            Mood Smoothing & Tracking
            Stabilizes predictions over time and logs mood trends for more consistent feedback
            Face Recognition (Simulated)
            Greets a configured user (e.g. “Charaf”) when a face is detected
            Dynamic Web Interface
            UI updates colors and animations based on detected emotions
            Smart Dashboard
            Live clock
            Weather integration (OpenWeather API)
            Emotion-based music playback
            Machine Learning Included
            Emotion model training script (emotion_model_best.h5)
            Experimental gesture recognition model (gesture_model_best.h5)
            
🛠️ Tech Stack
            Python
            Flask
            OpenCV
            TensorFlow / Keras
            HTML / CSS / JavaScript
            Raspberry Pi (Picamera2)
⚙️ Setup
1. Hardware
            Raspberry Pi
            Compatible camera module (Picamera2)
2. Model

Place your trained model at:

            /home/kip/SmartMirror/emotion_model_best.h5

            (or update the path in api_server_stream.py)

3. API Key

Add your OpenWeather API key in:

            index.html

4. Run
            python3 api_server_stream.py

Open in browser:

http://<YOUR_PI_IP>:5000

📌 Notes

Designed for local network use
Performance depends on Raspberry Pi model
Emotion detection accuracy varies with lighting and camera quality
