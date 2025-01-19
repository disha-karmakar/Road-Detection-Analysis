
# Road Detection Analysis

This repository contains a comprehensive analysis of the **Road_Related_Classes-IMGs&Labels** dataset using a YOLO-based object detection model. The project aims to detect road-related objects such as traffic lights, stop signals, speed limit signs, and vehicles from images.

## Table of Contents
- [Road Detection Analysis](#road-detection-analysis)
  - [Table of Contents](#table-of-contents)
  - [Overview](#overview)
  - [Dataset](#dataset)
  - [Key Features](#key-features)
  - [YOLO Model](#yolo-model)
  - [Installation and Setup](#installation-and-setup)
  - [Usage](#usage)
  - [Results](#results)
  - [License](#license)

---

## Overview

Road object detection is a critical task for autonomous vehicles, traffic monitoring systems, and urban planning. This project leverages the **YOLO (You Only Look Once)** architecture to perform efficient and accurate object detection on road-related images.

---

## Dataset

The **Road_Related_Classes-IMGs&Labels** dataset includes:
- **Classes**:
  - Traffic Light Signal
  - Stop Signal
  - Speed Limit Signal
  - Crosswalk Signal
  - Crosswalk
  - Pedestrian
  - Bus
  - Car
  - Truck
- **Structure**:
  - Train, Validation, and Test splits.
  - Images paired with `.txt` files containing annotations in YOLO format.

---

## Key Features

1. **Dataset Exploration**:
   - Validates the dataset for consistency (e.g., matching image-label pairs).
   - Visualizes the class distribution using bar charts and word clouds.

2. **Data Preprocessing**:
   - Resizes images to `(128, 128)` and normalizes pixel values.
   - Splits data into training and validation sets.
   - Applies data augmentation (rotation, zoom, etc.) for better generalization.

3. **YOLO-based Model**:
   - Trains a YOLO model for detecting road-related objects.
   - Fine-tunes parameters for optimal performance.

4. **Evaluation**:
   - Computes metrics like mAP, precision, and recall.
   - Visualizes predictions using bounding boxes overlaid on images.

5. **Summary and Conclusion**:
   - Provides key insights from the analysis.
   - Suggests potential improvements and future directions.

---

## YOLO Model

The YOLO (You Only Look Once) architecture is designed for real-time object detection. Key highlights:
- **Efficiency**: Processes images in a single forward pass.
- **Accuracy**: Balances precision and speed, making it ideal for real-world applications.
- **Customizability**: Supports anchor box adjustments for specific datasets.

---

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/disha-karmakar/Road-Detection-Analysis.git
   cd Road-Detection-Analysis
   ```

2. **Install Dependencies**:
   Create a Python virtual environment and install the required libraries:
   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Open the Notebook**:
   Launch Jupyter Notebook or your preferred environment:
   ```bash
   jupyter notebook Road_Detection_Analysis.ipynb
   ```

---

## Usage

1. **Dataset Preparation**:
   - Ensure the dataset is available in the specified directory structure.

2. **Run the Notebook**:
   - Execute the cells step by step for data exploration, model training, and evaluation.

3. **View Results**:
   - Inspect evaluation metrics and predictions in the output cells.

---

## Results

The YOLO model demonstrated promising results:
- **mAP**: Achieved high accuracy in detecting road-related objects.
- **Visualization**: Detected objects are overlaid with bounding boxes on images.

---

## License

This project is licensed under the [MIT License](LICENSE).
