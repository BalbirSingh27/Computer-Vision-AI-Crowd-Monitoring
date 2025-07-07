# 🧠 Real-Time Crowd Detection Using Computer Vision at ASU Gym

## 📌 Project Overview

This project showcases a real-time gym crowd monitoring system using **Computer Vision (CV)** to enhance student experience and optimize gym utilization at **Arizona State University (ASU)**. It leverages classic CV techniques like **HOG + SVM** to detect people in images and generates **animated heatmaps** to visualize gym occupancy trends.

> 🛠 Developed as part of the **CIS 515: Computer Vision and AI** course at [ASU](https://www.asu.edu), by Team008.

---

## 🎯 Objective

- Detect individuals in gym surveillance images  
- Generate visual heatmaps showing crowd density  
- Support students in choosing optimal gym hours  
- Lay the foundation for a scalable, real-time deployment

---

## 📂 Dataset

The project uses open-source crowd images from Kaggle and simulated gym-like frames.

📊 **Dataset Used**:  
[Kaggle – Crowd Counting Dataset by Balbir](https://www.kaggle.com/datasets/balbir27/ai-crowd-monitoring)

---

## 🛠 Technologies Used

- **Language**: Python  
- **Libraries**: OpenCV, NumPy, Seaborn, Matplotlib, OS  
- **Model**: Histogram of Oriented Gradients (HOG) + Support Vector Machine (SVM)  
- **Task**: Pedestrian detection on static images  
- **Output**: Heatmaps for each frame + animated GIF showing density patterns

---

## 🧪 Methodology

1. **Image Preprocessing**
   - Images resized and converted to RGB
   - Normalization applied for detection optimization

2. **Person Detection**
   - OpenCV’s `hog.detectMultiScale()` used to detect people
   - Detections stored per frame for visualization

3. **Heatmap Generation**
   - Seaborn heatmaps created based on bounding box coordinates
   - Combined into a single animated crowd GIF

4. **Evaluation**
   - Compared detections with ground truth counts
   - MAE (Mean Absolute Error) ≈ 20 people per frame

---

## 📽 Sample Outputs

- ✔️ Detected people with bounding boxes  
- ✔️ Individual heatmap per frame  
- ✔️ Animated GIF showing overall crowd flow

---

## ⚖️ Evaluation Summary

| Metric              | Result             |
|---------------------|--------------------|
| MAE (avg. error)    | ~20 people/frame   |
| Detection Accuracy  | Moderate (baseline model) |
| Processing Speed    | Real-time capable  |

---

## 🔐 Privacy & Ethics

- No actual ASU gym footage or personal data used  
- Project used anonymized and synthetic crowd datasets  
- Future improvements will include real-time anonymization methods

---

## 🚀 Future Enhancements

- Integrate **YOLOv8** or **MobileNet SSD** for better accuracy in dense crowds  
- Stream real-time video from gym cams  
- Deploy heatmap dashboard in a **mobile app for students**  
- Expand to all ASU athletic facilities  
- Add REST APIs for live data sharing

---

## 👥 Team Contributions

| Name             | Contributions                                     |
|------------------|----------------------------------------------------|
| **Balbir Singh** | Evaluation metrics, risk mitigation, final review |
| Maria Sequeira   | Detection pipeline, OpenCV logic                  |
| Rasika Teli      | Dataset preparation, problem formulation         |
| Yu Chin Chen     | Heatmap generation, model tuning                 |
| Harsh Kevadiya   | Project limitations, roadmap, presentation design|

---

## 🔗 Useful Links

## 📎 Reference Links

🔗  ## 📎 Reference Links

## 📎 Reference Links

🧠 [OpenCV People Detection Script](https://github.com/opencv/opencv/blob/4.x/samples/python/peopledetect.py)  
📚 [Histogram of Oriented Gradients – LearnOpenCV](https://learnopencv.com/histogram-of-oriented-gradients/)  
🏋️ [RecWell at UC Berkeley](https://recwell.berkeley.edu/recreation-wellbeing-program-and-service-updates/)  
📱 [RU Gyms Crowd Meter – Devpost](https://devpost.com/software/ru-gyms-crowd-meter)  
📊 [Kaggle Dataset](https://www.kaggle.com/datasets/balbir27/ai-crowd-monitoring)

---

## 🏷 Tags

`#ComputerVision` `#OpenCV` `#CrowdMonitoring` `#GymAnalytics`  
`#HOG` `#ASU` `#Python` `#Heatmap` `#CIS515` `#Team008`
