# Carbon-Aware Green Traffic Monitoring Using Motion-Based Deep Learning Model Scheduling

## 📌 Overview

We developed a motion-based traffic monitoring framework that activates deep learning-based vehicle detection only when motion is detected. By integrating a **Gaussian Mixture-based Background Subtraction (MOG2)** motion detection mechanism, our framework avoids unnecessary inference during inactive scenes, reducing energy consumption and carbon emissions while maintaining effective traffic monitoring performance.

Our approach explores energy-aware scheduling across multiple object detection models to make intelligent and environmentally sustainable traffic monitoring more practical.

## 🎯 Key Contributions

- **Motion-Based Scheduling:** Runs the object detector only when motion is detected.
- **Energy Efficiency:** Reduces unnecessary deep learning inference.
- **Carbon-Aware Monitoring:** Evaluates the environmental impact of model execution.
- **Multi-Model Evaluation:** Compares different object detection architectures under the proposed scheduling strategy.
- **Performance Analysis:** Evaluates detection performance alongside energy consumption, power usage, carbon emissions, and computational cost.

## 🧠 Models Evaluated

The framework evaluates the following object detection models:

- YOLOv8n
- YOLOv9c
- YOLOv11n
- YOLO26n
- RT-DETR-L

## ⚙️ Methodology

1. **Video Input:** Receives traffic video frames for monitoring.
2. **Motion Detection:** Uses MOG2 background subtraction to identify motion.
3. **Model Scheduling:** Activates the selected deep learning detector when motion is detected.
4. **Vehicle Detection:** Detects vehicles in relevant frames.
5. **Environmental Evaluation:** Measures detection performance and energy-related metrics.
6. **Comparison:** Compares scheduled inference with conventional inference without motion-based scheduling.

## 📊 Key Results

The proposed framework achieved the following reported reductions:

| Metric | Maximum Reduction |
|---|---:|
| Energy Consumption | 80.52% |
| Carbon Emissions | 85.72% |

These results demonstrate the potential of motion-based model scheduling to improve the energy efficiency and environmental sustainability of deep learning-based traffic monitoring.

## 🛠️ Technologies

- Python
- OpenCV
- PyTorch
- YOLO-based object detection
- RT-DETR
- MOG2 Background Subtraction

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone <YOUR_REPOSITORY_URL>
cd <YOUR_REPOSITORY_FOLDER>
```

### 2. Install Dependencies

Create and activate a Python virtual environment if needed, then install the required packages.

```bash
pip install opencv-python torch ultralytics
```

Install any additional dependencies required by your implementation, including those needed for RT-DETR and energy measurement.

### 3. Run the Project

Run the relevant inference or evaluation script using your traffic video dataset and selected detection model.

> **Note:** Update this section with the actual script names, dataset paths, and configuration options used in your repository.

## 📁 Suggested Repository Structure

```text
.
├── datasets/
├── models/
├── scripts/
│   ├── motion_detection.py
│   ├── traffic_detection.py
│   └── evaluation.py
├── results/
├── requirements.txt
└── README.md
```

*This is a suggested structure. Adapt it to match the actual repository files.*

## 🌱 Impact

This project explores a practical approach to **Green AI** by reducing unnecessary computation in traffic monitoring systems. Motion-aware scheduling can help make continuous video analytics more energy-efficient and reduce the environmental footprint of deep learning inference.

## 📄 Publication

**Title:** Carbon-Aware Green Traffic Monitoring using Motion-based Deep Learning Model Scheduling

Add the publication link, conference or journal details, and DOI here when available.

## 👥 Authors

**Md Noman Hossain** and collaborators.

Update this section with the complete author list and affiliations.

## 📜 License

Add the license applicable to this project. If you intend to release the code publicly, choose an appropriate open-source license.

## 🙏 Acknowledgements

We acknowledge the researchers and developers whose open-source computer vision frameworks made this work possible.
