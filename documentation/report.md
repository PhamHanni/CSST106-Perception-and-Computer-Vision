# Object Detection for Chair Detection Using SSD, HOG-SVM, and YOLO

**Authors:** Andrel John M. Pantanoza and Renato Elbo of BSCS-4A, CSST106-PERCEPTION-AND-COMPUTER-VISION

This document provides an overview and implementation details of three object detection techniques (SSD, HOG-SVM, and YOLO) used for detecting chairs in images.

---

## SSD Object Detection

### 1. Introduction
SSD (Single Shot MultiBox Detector) is an object detection algorithm that uses a single deep neural network to detect objects within an image. SSD is designed to identify objects of various sizes by making predictions at multiple scales.

### 2. Requirements
- TensorFlow/Keras
- OpenCV
- NumPy

### 3. Dataset
The dataset contains labeled images of chairs in various orientations and backgrounds, which enables the model to generalize well across different scenes.

### 4. Model Training
- **Model Initialization**: SSD model is based on the VGG-16 architecture for feature extraction.
- **Training Process**: The model is trained with a combination of localization and confidence loss.
- **Hyperparameters**:
  - Learning Rate: 0.001
  - Batch Size: 32
  - Epochs: 100

### 5. Evaluation
Performance metrics include accuracy, precision, recall, and F1-score to measure detection accuracy on test images.

### 6. Results
The SSD model demonstrates high accuracy with minimal false positives and negatives, effectively detecting chairs in various contexts.

### 7. Inference
- Load a test image.
- Run the model to obtain bounding box predictions.
- Display or save the result with detected chairs highlighted.

### Conclusion
SSD is a fast and accurate model, suitable for real-time applications that require chair detection.

---

## HOG-SVM for Chair Detection

### 1. Introduction
HOG-SVM uses a feature-based approach with Histogram of Oriented Gradients (HOG) to detect shapes and textures, making it suitable for detecting well-defined objects like chairs.

### 2. Requirements
- Scikit-learn
- OpenCV
- NumPy

### 3. Dataset
The dataset includes grayscale images of chairs, pre-processed to improve feature extraction.

### 4. HOG Feature Extraction
- **Parameters**:
  - Cell Size: 8x8
  - Block Size: 2x2 cells
  - Number of Bins: 9

### 5. SVM Classification
- **Hyperparameters**:
  - Kernel: Linear
  - Regularization Parameter (C): 1.0

### 6. Evaluation
Evaluation includes metrics such as accuracy, precision, and recall.

### 7. Results
The HOG-SVM model achieves high accuracy but may have limitations with occluded or low-contrast images.

### 8. Inference
1. Load a test image.
2. Extract HOG features.
3. Classify using SVM to detect chairs.

### Conclusion
HOG-SVM provides good accuracy for objects with clear features, but it requires more computation time compared to other methods.

---

## YOLO Object Detection

### 1. Introduction
YOLO (You Only Look Once) is a convolutional neural network-based model that processes the entire image in a single pass, making it highly efficient for real-time applications.

### 2. Requirements
- Darknet (for YOLO) or PyTorch (YOLOv5)
- OpenCV
- NumPy

### 3. Dataset
A labeled dataset of chair images with various orientations, sizes, and backgrounds is used.

### 4. Model Training
- **YOLO Architecture**: Divides the image into a grid and predicts bounding boxes and class probabilities.
- **Hyperparameters**:
  - Learning Rate: 0.001
  - Batch Size: 16
  - Epochs: 50

### 5. Evaluation
- **Metrics**: Mean Average Precision (mAP) and Precision-Recall curve.

### 6. Results
YOLO achieves high-speed and accurate chair detection, making it suitable for real-time applications.

### 7. Inference
1. Load an image.
2. Run the YOLO model for bounding box predictions.
3. Display or save the image with detected chairs highlighted.

### Conclusion
YOLO balances speed and accuracy, making it ideal for real-time chair detection applications.

---

## Overall Conclusion
This document outlines three different approaches to chair detection—SSD, HOG-SVM, and YOLO—each with unique strengths. SSD and YOLO are suitable for real-time applications due to their speed, while HOG-SVM provides accurate results for clear, well-defined objects but is less efficient in processing speed.

**Authors:** Andrel John M. Pantanoza and Renato Elbo of BSCS-4A, CSST106-PERCEPTION-AND-COMPUTER-VISION
