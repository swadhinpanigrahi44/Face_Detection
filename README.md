# Face Detection & Recognition System 🎯

A real-time **face detection and face recognition system** built using **Python**, **OpenCV**, and a **deep learning model (Keras)**.  
The project captures face data, preprocesses images, trains a model, and performs live face recognition using a camera stream.

---

## 🚀 Features
- 📷 Real-time face capture using IP camera
- 🧠 Face detection using Haar Cascade (OpenCV)
- 🗂 Automatic dataset creation (100 images per person)
- 🖤 Image preprocessing (grayscale, resize, normalization)
- 🤖 Face recognition using a trained deep learning model (`.h5`)
- 🧾 Label-based identity prediction
- 🔴 Live bounding box and name display

---

## 🛠 Tech Stack
- **Python**
- **OpenCV**
- **NumPy**
- **Keras / TensorFlow**
- **Pickle**
- **IP Webcam (mobile camera stream)**

---

## 📁 Project Structure
Face_Detection/
│
├── collect_data.py # Capture and store face images
├── consolidated_data.py # Preprocess and serialize data
├── recognize.py # Real-time face recognition
├── final_model.h5 # Trained deep learning model
├── haarcascade_frontalface_default.xml
├── images/ # Captured face images (ignored in git)
├── data/
│ ├── images.p
│ └── labels.p
└── .gitignore

---

## 📸 Data Collection
Run the script to capture **100 face images** for a person: python collect_data.py

-Uses Haar Cascade to detect faces
-Saves images as: name_index.jpg
-Stores images in the images/ folder

---

## 🧪 Data Preprocessing
Convert images into training-ready format: python consolidated_data.py

-Resizes images to 100x100
-Converts to grayscale
-Saves processed data using Pickle

---

## 🧠 Face Recognition (Live)
Start real-time recognition: python recognize.py

-Detects faces in live video stream
-Predicts identity using trained model
-Displays name with bounding box

---

## ⚙️ Requirements
Install dependencies:

pip install opencv-python numpy tensorflow keras matplotlib

---

## ⚠️ Notes

-Update IP camera URL in scripts before running
-Ensure Haar Cascade and model paths are correct
-Labels list in recognize.py must match trained classes

---

## 🧰 Development Tools
- Spyder IDE (Anaconda)
- Jupyter Notebook
- Python 3.x

---

## 👨‍💻 Author

Swadhin Panigrahi
Computer Science & Technology Student | Python & Computer Vision Enthusiast.
