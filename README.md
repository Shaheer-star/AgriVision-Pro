# AgriVision Pro: Edge-Optimized AI for Real-Time Crop Disease Diagnostics 🌾

![Python](https://img.shields.io/badge/Python-3.12-blue)
![TensorFlow](https://img.shields.io/badge/TensorFlow-Lite-orange)
![FastAPI](https://img.shields.io/badge/FastAPI-Backend-green)
![Docker](https://img.shields.io/badge/Docker-Deployment-blue)
![Status](https://img.shields.io/badge/Status-Live-brightgreen)

AgriVision Pro is an AI-powered crop disease detection system designed to help users identify plant diseases from leaf images in real time. The project combines deep learning, TensorFlow Lite optimization, and a modern FastAPI-based web application to make crop health diagnosis faster, simpler, and more accessible.

The system supports **38 plant disease and healthy classes** across multiple crop categories and provides prediction results with confidence scores and treatment recommendations through an interactive web interface.

---

## 🌐 Live Project & Documentation

🚀 **Live Demo:** Add your Hugging Face Space link here  
📄 **Project Documentation:** [AgriVision Pro Documentation](https://agrivision-pro-u2w7jqp.gamma.site/)  
💻 **GitHub Repository:** [AgriVision-Pro](https://github.com/Shaheer-star/AgriVision-Pro)  
👤 **LinkedIn:** [Syed Shaheer Abbas](https://www.linkedin.com/in/syed-shaheer-abbas/)

---

## 📌 Project Overview

Crop diseases can spread quickly and cause serious agricultural losses if not detected early. Many farmers and students do not have immediate access to plant pathology experts, especially in remote areas.

AgriVision Pro solves this problem by allowing users to upload a crop leaf image and instantly receive:

- predicted plant disease
- crop/plant name
- confidence score
- treatment recommendations
- modern visual result display

This project demonstrates how **AI vision**, **edge optimization**, and **web deployment** can be combined to build practical smart agriculture tools.

---

## 🚀 Key Features

### 🌿 38 Disease Classes

AgriVision Pro supports classification across 38 healthy and diseased plant categories based on the PlantVillage-style disease class structure.

### ⚡ Real-Time Prediction

Users can upload a leaf image and receive near-instant disease prediction results through the web interface.

### 📱 Edge-Optimized Model

The trained deep learning model is converted into **TensorFlow Lite `.tflite` format**, making it lightweight and suitable for faster inference and future mobile or IoT deployment.

### 🧠 AI-Powered Diagnosis

The system analyzes visible patterns such as:

- leaf spots
- discoloration
- mold
- rust
- blight
- bacterial symptoms
- viral disease patterns

### 🖥️ Modern Interactive Interface

The frontend includes:

- animated AI dashboard design
- drag-and-drop image upload
- image preview
- scanning animation
- confidence progress bar
- disease result card
- treatment recommendation cards

### 🩺 Treatment Recommendations

After prediction, the app provides disease-specific treatment suggestions to guide users toward possible next actions.

### 🐳 Deployment Ready

The project includes Docker support and can be deployed on platforms such as Hugging Face Spaces.

---

## 🛠️ Technical Stack

| Category | Technology |
|---|---|
| Programming Language | Python |
| Deep Learning Framework | TensorFlow / Keras |
| Model Format | TensorFlow Lite |
| Backend Framework | FastAPI |
| Server | Uvicorn |
| Image Processing | Pillow, NumPy |
| Frontend | HTML, CSS, JavaScript |
| Deployment | Docker, Hugging Face Spaces |
| Documentation | Gamma |

---

## 🧠 Model Information

| Item | Details |
|---|---|
| Task Type | Multi-class image classification |
| Supported Classes | 38 |
| Input Type | RGB crop leaf image |
| Input Size | 224 × 224 |
| Model Format | `.tflite` |
| Inference Engine | TensorFlow Lite Interpreter |
| Backend API | FastAPI `/predict` endpoint |

> Note: Add actual training and validation accuracy after evaluating the model with your final test dataset.

---

## 🌱 Supported Disease Categories

AgriVision Pro supports common crop disease and healthy categories from multiple crops, including:

- Apple
- Blueberry
- Cherry
- Corn / Maize
- Grape
- Orange
- Peach
- Bell Pepper
- Potato
- Raspberry
- Soybean
- Squash
- Strawberry
- Tomato

Examples of detected conditions include:

- Apple Scab
- Apple Black Rot
- Cedar Apple Rust
- Corn Common Rust
- Corn Northern Leaf Blight
- Grape Black Rot
- Potato Early Blight
- Potato Late Blight
- Tomato Early Blight
- Tomato Late Blight
- Tomato Leaf Mold
- Tomato Mosaic Virus
- Tomato Yellow Leaf Curl Virus
- Strawberry Leaf Scorch
- Squash Powdery Mildew

---

## 🔍 How It Works

### 1. Image Upload

The user uploads a crop leaf image through the web interface.

### 2. Image Preprocessing

The backend processes the image by:

- reading the uploaded file
- converting it to RGB
- resizing it to the model input size
- normalizing pixel values
- adding batch dimension

### 3. TensorFlow Lite Inference

The `.tflite` model is loaded using TensorFlow Lite Interpreter and performs prediction on the processed image.

### 4. Disease Classification

The system identifies the most likely disease class and calculates the confidence score.

### 5. Result Display

The frontend displays:

- plant name
- disease name
- confidence percentage
- treatment recommendations

---

## 🖥️ Application Interface

AgriVision Pro is designed with a modern AI dashboard interface. The UI includes a futuristic agriculture theme with animated elements, glassmorphism cards, drag-and-drop upload functionality, image preview, scanning effect, and visually clear prediction results.

Main interface features:

- responsive layout
- animated background
- crop-health dashboard cards
- upload area
- prediction result section
- confidence bar
- treatment plan cards

---

## 📁 Project Structure

```text
AgriVision-Pro/
│
├── main.py
├── requirements.txt
├── Dockerfile
├── README.md
├── .gitignore
├── .dockerignore
│
├── models/
│   └── crop_dignostic_edge_model.tflite
│
└── static/
    ├── index.html
    ├── farmpic.jpg
    └── favicon.png
