# AgroVision

### Drone-Based Agricultural Field Classification using Deep Learning

AgroVision is a computer vision system that classifies agricultural fields from drone imagery using **Transfer Learning with ResNet50**. The project demonstrates how aerial data and deep learning can support **precision agriculture**, automated land analysis, and scalable farm monitoring.

---

## Problem Statement

Large-scale agricultural monitoring is time-consuming and resource-intensive when done manually. With the increasing use of drones in farming, there is a need for intelligent systems that can automatically analyze aerial images and classify different types of agricultural fields.

AgroVision addresses this problem by building a deep learning model that learns field patterns directly from drone-captured images.

---

## Key Features

* Agricultural field classification from drone images
* Transfer learning using pretrained **ResNet50**
* Automated image preprocessing pipeline
* Model training and validation
* Performance visualization (accuracy & loss)
* Scalable architecture for real-world deployment

---

## Dataset

**Drone Camera Image Dataset of Agriculture Fields**

Kaggle:
https://www.kaggle.com/datasets/suhelahamed/drone-camera-image-dataset-of-agriculture-fields

### Dataset Characteristics

* Drone-captured aerial field images
* Multiple agricultural land categories
* Real-world variations in texture, pattern, and lighting

> The dataset is not included in this repository due to size limitations.

### After Download, Place Dataset Here

```
AgroVision/
│
├── data/
│   ├── class_1/
│   ├── class_2/
│   └── ...
```

---

## Project Structure

```
AgroVision/
│
├── notebook/
│   └── minor-project-1-0(1).ipynb
│
├── data/              # Download from Kaggle
├── models/            # Saved model weights 
│   └── best_model.h5
├── requirements.txt
├── README.md
└── .gitignore
```

---

## Technology Stack

* Python
* TensorFlow / Keras
* ResNet50 (ImageNet pretrained)
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Scikit-learn

---

## Model Pipeline

1. Load drone images
2. Resize and normalize images
3. Train-validation split
4. Load pretrained ResNet50 (without top layer)
5. Add custom classification layers
6. Train using transfer learning
7. Evaluate model performance

---

## Installation

### 1. Clone Repository

```
git clone https://github.com/your-username/AgroVision.git
cd AgroVision
```

### 2. Install Dependencies

```
pip install -r requirements.txt
```

### 3. Download Dataset

Download from Kaggle and place inside:

```
AgroVision/data/
```

---

## How to Run

Launch the notebook:

```
jupyter notebook notebook/AgroVision.ipynb
```

Run all cells sequentially.

---

## Results

The model outputs:

* Training accuracy and validation accuracy
* Loss curves
* Classification performance
* Predictions on unseen agricultural images

---

## Applications

* Precision agriculture
* Land-use classification
* Crop monitoring
* Agricultural surveys
* Smart farming systems

---

## Future Enhancements

* Web application for image upload and prediction
* Real-time drone feed analysis
* Crop health and disease detection
* Model optimization for edge devices
* Deployment using TensorFlow Lite or FastAPI

---

## Author

**AVIK HALDER**
GitHub: [https://github.com/avikxr387](https://github.com/avikxr387)

---

## License

MIT License
