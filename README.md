# 🚗 Robust Object Detection in ADAS Using Video Dehazing Under Adverse Weather Conditions

This repository contains the code, datasets, and documentation for a deep learning-based Advanced Driver Assistance System (ADAS) that improves object detection under low-visibility conditions such as haze, fog, and rain. It combines video dehazing using LightClearNet with real-time object detection using YOLOv11.

---

## 📌 Problem Statement

Develop a deep learning-based system that dehazes/enhances images and videos while simultaneously detecting objects using the YOLO architecture to improve detection accuracy in challenging weather conditions.

---

## 🎯 Objectives

- 🔧 Develop a deep learning model to enhance hazy images and videos.
- 🤖 Integrate image enhancement with YOLO for object detection.
- 🧪 Train and test on hazy datasets for robust performance.
- 🎯 Improve detection accuracy under low-visibility conditions.
- ⏱ Build a real-time capable pipeline for ADAS and surveillance systems.

---

## 🛠️ Methodology

1. **Dehazing**: LightCleanNet, a lightweight encoder-decoder model, is used to dehaze video frames.
2. **Preprocessing**: Brightness and contrast are enhanced post-dehazing.
3. **Object Detection**: YOLOv11 is applied to the dehazed frames for robust object detection.
4. **Postprocessing**: Objects are annotated and frames are saved.
5. **Temporal Consistency**: Optical flow smoothing is applied to ensure visual consistency.
6. **Evaluation**: PSNR, SSIM, and mAP@0.5 are computed to measure performance.

---

## 📂 Project Structure

```
├── dehazing/
│   └── lightclearnet_model.py
├── detection/
│   └── yolov11_inference.py
├── data/
│   ├── input_videos/
│   └── output_videos/
├── utils/
│   └── metrics.py
├── results/
│   └── sample_outputs/
├── README.md
└── requirements.txt
```

---

## 📊 Results

| Model          | PSNR (dB) | SSIM   | 
|----------------|-----------|--------|
| LightClearNet  | 21.17     | 0.852  | 
| Our Project    | 28.08     | 0.632  | 

Detection accuracy improved by **51.94%** over hazy inputs.

### Evaluation Metrics of YOVO V11:

❏	Hazy Video mAP@0.5: 0.4523

❏	Dehazed Video	mAP@0.5: 0.6872

❏	Detection Improvement: 0.2349 (51.94%)


---

## 📚 Literature Survey

- **LightClearNet**: Lightweight encoder-decoder for real-time dehazing using CNNs.
- **YOLOv11**: Improved real-time object detector suitable for adverse weather ADAS applications.

---

## 📦 Dataset Used

- **RESIDE-6K**: 6,000 hazy/clear image pairs for training and 1,000 pairs for testing (indoor and outdoor scenes).

---

## 🧪 Evaluation Metrics

- **PSNR (Peak Signal-to-Noise Ratio)**
- **SSIM (Structural Similarity Index)**
- **mAP@0.5 (Mean Average Precision at 0.5 IOU)**

---

## ✅ Contributions

- Real-time video dehazing with a lightweight model.
- Integration with YOLOv11 for robust object detection.
- Avoids heavy models like transformers to ensure fast execution.
- Temporal smoothing with optical flow for video consistency.

---

## 🧑‍💻 Authors

- Bhoomika Hosamani – [01fe22bec240@kletech.ac.in](mailto:01fe22bec240@kletech.ac.in)  
- Ankita Angadi – [01fe22bec246@kletech.ac.in](mailto:01fe22bec246@kletech.ac.in)  
- Chandana Janmatti – [01fe22bec267@kletech.ac.in](mailto:01fe22bec267@kletech.ac.in)  
- Shreedevi Angadi – [01fe22bec288@kletech.ac.in](mailto:01fe22bec288@kletech.ac.in)  

---

## 👩‍🏫 Guide

Prof. Rajeshwari K, Department of ECE, KLE Technological University.

---

## 📌 Future Scope

- Extend to night-to-day translation for low-light driving.
- Deploy on embedded devices for real-time ADAS integration.
- Incorporate sensor fusion with radar or LiDAR for improved safety.

---

## 📄 License

This project is licensed under the MIT License.

## PPT link
https://docs.google.com/presentation/d/19gaH1_juh7pDMrI6WWIfZb_4Y9M2yWWN/edit?usp=sharing&ouid=109979185302828264843&rtpof=true&sd=true

## POSTER link
https://docs.google.com/presentation/d/13kwQV4avBsmCGBgnclFPlQrOSmXA1G01/edit?usp=sharing&ouid=109979185302828264843&rtpof=true&sd=true
