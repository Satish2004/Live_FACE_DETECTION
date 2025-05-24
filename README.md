# Face Identifier – Python Project (OpenCV + AI/ML)

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

```bash
pip install opencv-python opencv-contrib-python numpy

📁 Project Structure
FaceIdentifier/
│
├── facecapture.py                   # Captures face images and assigns ID
├── trainer.py                       # Trains face recognizer model
├── recognizer.py                    # Detects and recognizes faces live
├── haarcascade_frontalface_default.xml  # Pre-trained face detection model
│
├── dataset/                         # Stores face images and names.txt
│   └── names.txt                    # Maps ID to names (e.g., 0,John)
│
├── trainer/                         # Stores trained recognizer model (.yml)

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

