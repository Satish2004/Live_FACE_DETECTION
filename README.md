# Live Face_DETECTION – Python Project (OpenCV + AI/ML)

This project is a simple Face Recognition system using Python, OpenCV, and the LBPH Face Recognizer. It captures images from your webcam, trains a recognizer model, and identifies faces in real-time.

---

## 🛠 Features

- Face detection using Haar cascades
- Face data collection and labeling
- Model training with OpenCV's LBPH
- Real-time face recognition via webcam

---

## 🖥️ Requirements

- Python 3.8 or higher  
- Webcam

### 📦 Install Dependencies

Open terminal/command prompt and run:

pip install opencv-python opencv-contrib-python numpy


🚀 Getting Started (Step-by-Step)
✅ Step 1: Install Python
Download from python.org

Check ✅ "Add Python to PATH" during install

Verify with:
python --version

✅ Step 2: Install Required Libraries
pip install opencv-python opencv-contrib-python numpy

✅ Step 3: Capture Face Images
python facecapture.py

1) Enter a unique numeric ID and name
2) Look at the webcam — captures ~100 samples
3) Saves images in dataset/ and name mapping in dataset/names.txt

✅ Step 4: Train the Model
python trainer.py

1) Trains the model using images in dataset/
2) Saves the trained model in trainer/trainer.yml


✅ Step 5: Run the Recognizer
python recognizer.py

1) Starts webcam
2) Detects and identifies faces
3) Displays the name and confidence level

🧠 Dataset Format
dataset/User.<id>.<count>.jpg
Name file (dataset/names.txt):
example->
0,John
1,Alice
2,Bob

![Image](https://github.com/user-attachments/assets/37ce69fd-88f1-4351-931d-d1a20f74d3f2)




