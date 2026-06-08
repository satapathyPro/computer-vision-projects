# Computer Vision Projects

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

A curated collection of computer vision projects that apply **transfer learning** and **convolutional neural networks (CNNs)** to real-world classification and detection tasks — spanning medical imaging, autonomous driving, and safety-critical applications.

---

## Projects

| Project | Task | Architecture / Model | Accuracy |
|---|---|---|---|
| Cataract Detection | Binary classification (cataract vs. normal) | Pretrained CNN + fine-tuning | See notebook |
| Traffic Sign Classification | Multi-class classification (43 classes) | CNN / Transfer Learning | See notebook |
| Pneumonia Detection | Binary classification from chest X-rays | Pretrained CNN + fine-tuning | See notebook |
| Driver Drowsiness Detection | Binary classification (drowsy vs. alert) | Transfer Learning + Parallel Conv Architecture | See notebook |
| Eye Disease Classification | Multi-class eye disease diagnosis | CNN with Parallel Convolution Architecture | See notebook |
| Emotion Detection | Multi-class facial emotion recognition | CNN | See notebook |
| MNIST Digit Classification | 10-class digit recognition | Custom CNN | See notebook |
| Lane Detection | Lane segmentation for autonomous vehicles | Computer vision pipeline (OpenCV) | — |
| Object Detection (YOLOv3) | Real-time multi-class object detection | YOLOv3 | See notebook |

---

## Why Transfer Learning?

Training deep CNN models from scratch requires millions of labeled images and significant compute. **Transfer learning** sidesteps this by starting from a model already pretrained on a large dataset (e.g., ImageNet) and fine-tuning it on a smaller, domain-specific dataset.

This is especially valuable in:

- **Medical imaging** (cataract detection, pneumonia detection, eye disease classification) — labeled medical data is scarce and expensive to annotate.
- **Traffic / safety tasks** (traffic sign detection, driver drowsiness) — pretrained feature extractors generalize well to new visual domains with minimal data.

The result: faster convergence, better generalization, and state-of-the-art accuracy even with limited training samples.

---

## Results

Performance metrics for each project are reported in their respective notebooks. Key highlights:

- **Cataract Detection** — Binary classifier trained on fundus images; fine-tuned pretrained backbone. See notebook for confusion matrix and ROC curve.
- **Traffic Sign Classification** — 43-class classifier on the GTSRB dataset using transfer learning. See notebook for per-class accuracy breakdown.
- **Pneumonia Detection** — Chest X-ray binary classifier. Fine-tuned pretrained model on NIH / Kaggle pneumonia dataset. See notebook for sensitivity/specificity metrics.
- **Driver Drowsiness Detection** — Real-time classification using a parallel convolution architecture for improved multi-scale feature extraction.
- **Eye Disease Classification** — Multi-class CNN with parallel convolution branches for diabetic retinopathy, glaucoma, and other conditions.
- **YOLOv3 Object Detection** — Real-time multi-object detection with bounding box regression and class confidence scores.

> All experiments are implemented as self-contained Jupyter notebooks with inline visualizations and metric summaries.

---

## Repository Structure

```
computer-vision-projects/
├── cataract-detection/
├── traffic-sign-detection/
├── pneumonia-detection/
├── driver-drowsiness-detection/
├── eye-diseases/
├── emotion-detection/
├── mnist-digit-classification/
├── lane-detection/
└── object-detection-yolov3/
```

---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/satapathyPro/computer-vision-projects.git
cd computer-vision-projects

# Install dependencies
pip install torch torchvision tensorflow opencv-python matplotlib numpy scikit-learn jupyter

# Open a project notebook
jupyter notebook cataract-detection/
```

Each project folder contains its own notebook with dataset instructions, model training code, and evaluation results.

---

## Tech Stack

| Tool | Purpose |
|---|---|
| PyTorch / TensorFlow | Model training and transfer learning |
| OpenCV | Image preprocessing and computer vision pipelines |
| Jupyter Notebook | Interactive experimentation and visualization |
| scikit-learn | Metrics, evaluation, and data splitting |
| Matplotlib / Seaborn | Result visualization |

---

## Maintainer

**Subham Satapathy** — Software Engineer with 6+ years of experience building cloud-scale distributed systems and machine learning pipelines. Specializes in computer vision, PyTorch, TensorFlow, and production-ready AI automation.

- GitHub: [satapathyPro](https://github.com/satapathyPro)
- LinkedIn: [subhamumd](https://www.linkedin.com/in/subhamumd/)
- Email: satapathypro@gmail.com
