# 🧠 Real-Time Crowd Detection Using Computer Vision at ASU Gym

## 📌 Project Overview

This project focuses on **real-time gym crowd monitoring** using **Computer Vision (CV)** to enhance student experience and promote efficient gym usage at Arizona State University (ASU). The system detects people in gym surveillance frames, generates animated heatmaps showing density levels, and helps students plan gym visits more effectively.

> 🔍 Built as part of the **CIS 515 Final Project** at [ASU](https://www.asu.edu), leveraging **OpenCV, HOG + SVM**, and image processing.

---

## 🎯 Objective

- Detect people in real-time gym video frames using CV  
- Generate crowd density heatmaps  
- Reduce overcrowding and save student time  
- Build a scalable framework for campus-wide deployment

---

## 🛠 Technologies Used

- **Language**: Python  
- **Libraries**: OpenCV, NumPy, Matplotlib, Seaborn, OS  
- **Model**: HOG (Histogram of Oriented Gradients) + SVM  
- **Computer Vision Task**: Pedestrian detection in static frames  
- **Output**: Heatmaps per frame + Animated GIF

---

## 🧪 Methodology

1. **Data Source**: Public crowd images from [Kaggle Crowd Counting Dataset](https://www.kaggle.com/datasets/fmena14/crowd-counting/data)
2. **Preprocessing**:
   - Resized and converted images to RGB
   - Normalized for OpenCV detection
3. **Detection**:
   - Applied OpenCV’s `hog.detectMultiScale()` to detect people
   - Stored detected coordinates per frame
4. **Heatmap Generation**:
   - Generated heatmaps with Seaborn based on detection counts
   - Saved per-frame heatmaps for compilation
5. **Evaluation**:
   - Compared predicted people counts with ground truth
   - MAE (Mean Absolute Error) ≈ 20 people per frame

---

## 📽 Sample Outputs

- ✅ Per-frame person detections  
- ✅ Heatmap images  
- ✅ Animated crowd density GIF

---

## ⚖️ Evaluation

| Metric            | Result              |
|-------------------|---------------------|
| MAE (avg error)   | ~20 people/frame    |
| Detection Accuracy| Moderate            |
| Performance       | Real-time viable    |

---

## 🔐 Privacy & Ethics

- No personal identifiers used  
- Only crowd-level metrics shown  
- Future versions will improve anonymization and efficiency

---

## 🌐 Future Work

- Switch to **YOLOv8** or **MobileNet SSD** for high-density accuracy  
- Embed live heatmap into a **mobile app**  
- Expand across other ASU gym facilities  
- Explore real-time video streaming and backend APIs

---

## 👨‍💻 Team Contributions

- **Balbir Singh**: Model evaluation, MAE calculation, risk analysis, presentation conclusion  
- **Maria Sequeira**: End-to-end pipeline, system design  
- **Rasika Teli**: Dataset processing, problem framing  
- **Yu Chin Chen**: CV model setup, heatmap generation  
- **Harsh Kevadiya**: Limitations, future scope, quality review

---

## 🗂 Repo Structure

## 🔗 Links

- [Kaggle Dataset Used](https://www.kaggle.com/datasets/fmena14/crowd-counting/data)
- [OpenCV Pedestrian Detection](https://github.com/opencv/opencv/blob/4.x/samples/python/peopledetect.py)
- [Histogram of Oriented Gradients – LearnOpenCV](https://learnopencv.com/histogram-of-oriented-gradients/)

---

## 🔍 Tags

`#ComputerVision` `#OpenCV` `#CrowdDetection` `#Heatmaps` `#GymAnalytics` `#ASU` `#Team008` `#Python`
