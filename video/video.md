# Project Summary: Object Detection of Chairs Using SSD, HOG-SVM, and YOLO

**Authors:** Andrel John M. Pantanoza and Renato Elbo of BSCS-4A, CSST106-PERCEPTION-AND-COMPUTER-VISION

## Overview
This project explores three object detection algorithms—SSD (Single Shot MultiBox Detector), HOG-SVM (Histogram of Oriented Gradients with Support Vector Machine), and YOLO (You Only Look Once)—for the purpose of detecting chairs in images. Each method offers unique advantages, from high-speed real-time detection to reliable accuracy in feature-based recognition.

## Project Objectives
1. **Evaluate different object detection techniques** for their effectiveness in identifying chairs.
2. **Compare speed and accuracy** across SSD, HOG-SVM, and YOLO to determine their suitability for different real-time applications.

## Methods
1. **SSD (Single Shot MultiBox Detector)**: Utilizes a single deep neural network to detect objects, making predictions at multiple scales for objects of various sizes.
2. **HOG-SVM**: Extracts gradient features to classify chair images, leveraging Support Vector Machine for accurate recognition based on shape and texture.
3. **YOLO (You Only Look Once)**: Processes the entire image in one pass, allowing for rapid, high-accuracy detection suitable for real-time applications.

## Results and Findings
- **SSD** provided balanced accuracy and speed, showing strong performance in detecting chairs without compromising processing time.
- **HOG-SVM** achieved high accuracy in detecting well-defined objects but had a slower processing speed, making it less suitable for real-time applications.
- **YOLO** demonstrated superior speed and detection accuracy, making it ideal for applications where real-time detection is essential.

## Conclusion
Each model has its strengths, with YOLO and SSD favoring real-time applications, while HOG-SVM is best suited for scenarios prioritizing accuracy over speed.

## Video Presentation
A detailed video presentation of this project, explaining the methodologies, results, and comparisons, is available at the following link: [Video Presentation on Google Drive](https://drive.google.com/file/d/1AzqyOpjC32mMAs8TS71990NyNpopEmlh/view?usp=sharing)

---

This summary highlights the key aspects of the project, with the video link provided for a deeper look into the implementation and results.
