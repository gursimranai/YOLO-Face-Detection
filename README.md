# Object and Face Detection using YOLO & OpenCV

<p align="center">
  <b>A hands-on Computer Vision project exploring object detection, face detection, and real-time visual processing using Python, OpenCV, and YOLO models.</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-green?logo=opencv&logoColor=white" alt="OpenCV">
  <img src="https://img.shields.io/badge/YOLO-Object%20Detection-purple" alt="YOLO">
  <img src="https://img.shields.io/badge/PyTorch-Deep%20Learning-red?logo=pytorch&logoColor=white" alt="PyTorch">
  <img src="https://img.shields.io/badge/Jupyter-Notebooks-orange?logo=jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/Status-In%20Progress-yellow" alt="Project Status">
</p>

---

## About the Project

**Object and Face Detection using YOLO & OpenCV** is a practical Computer Vision project focused on exploring and implementing object detection and face detection techniques using pretrained deep learning models.

The project uses Python, OpenCV, Ultralytics YOLO, and other computer vision tools to experiment with image-based detection, real-time webcam detection, and different model configurations.

It also explores the integration of multiple detection models, CPU and GPU inference, and the practical applications of modern object detection systems.

This repository serves as a continuous learning and experimentation space where different models, techniques, and computer vision approaches can be implemented, tested, and documented.

## Project Objectives

- Understand the fundamentals of object detection and face detection.
- Explore different pretrained YOLO models and their architectures.
- Perform object and face detection on static images.
- Implement real-time detection using webcam streams.
- Experiment with multiple models in a single detection pipeline.
- Understand image and video processing using OpenCV.
- Explore CPU and GPU-based model inference.
- Evaluate detection performance and experiment with different configurations.
- Build practical experience with Computer Vision and Deep Learning.

## Technologies & Tools

| Technology | Purpose |
|---|---|
| Python | Primary programming language |
| OpenCV | Image processing, video capture, and visualization |
| Ultralytics YOLO | Object detection and model inference |
| YOLO Face | Face detection experiments |
| PyTorch | Deep learning framework |
| CUDA | NVIDIA GPU acceleration |
| NumPy | Numerical operations and image arrays |
| Matplotlib | Image visualization |
| Jupyter Notebook | Experimentation and documentation |

## Models & References

This project explores pretrained models from different open-source computer vision repositories.

### 1. General Object Detection

**Ultralytics YOLO**

Used for detecting general object categories such as people, animals, vehicles, and other supported objects.

- Repository: https://github.com/ultralytics/ultralytics
- Documentation: https://docs.ultralytics.com/

### 2. Face Detection

**YOLO Face — akanametov**

An open-source YOLO-based face detection implementation used for experimenting with face detection.

- Repository: https://github.com/akanametov/yolo-face

Different model variants can be explored depending on the experiment.

**Attribution:** Original model implementations and pretrained weights belong to their respective authors. This repository uses them for learning and experimentation and does not claim ownership of the original models.

## Project Structure

```text
SimpleFaceDetection/
│
├── assets/
│   ├── demo-images/
│   ├── screenshots/
│   └── videos/
│
├── notebooks/
│   ├── 01-image-detection.ipynb
│   ├── 02-webcam-detection.ipynb
│   ├── 03-cpu-vs-gpu-experiments.ipynb
│   └── 04-additional-model-experiments.ipynb
│
├── models/
│   └── README.md
│
├── experiments/
│   └── README.md
│
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

*The notebook list represents the planned organization and will expand as new experiments are added.*

## Getting Started

Follow these steps to set up the project locally.

### Prerequisites

- Python 3.10 or a compatible Python version supported by the selected dependencies.
- pip package manager.
- VS Code or Jupyter Notebook.
- Webcam (for real-time detection experiments).
- NVIDIA GPU with compatible CUDA support (optional).

### 1. Clone the Repository

```bash
git clone https://github.com/gursimranai/SimpleFaceDetection.git
```

### 2. Navigate to the Project Directory

```bash
cd SimpleFaceDetection
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

### 4. Activate the Environment

**Windows PowerShell:**

```powershell
.\.venv\Scripts\Activate.ps1
```

### 5. Install Dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 6. Install PyTorch with CUDA (Optional)

For NVIDIA GPU acceleration, install a compatible PyTorch build by following the official installation instructions:

https://pytorch.org/get-started/locally/

Verify CUDA availability:

```python
import torch

print("CUDA Available:", torch.cuda.is_available())

if torch.cuda.is_available():
    print("GPU:", torch.cuda.get_device_name(0))
```

### 7. Obtain Model Weights

Download the required pretrained model weights from their respective original repositories.

Examples:

- `yolov8n.pt`
- `yolov8m-face.pt`

Model weights are excluded from Git tracking because of their file size. Keep them in the project root or another appropriate local directory and configure the notebook paths accordingly.

### 8. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the notebooks inside the `notebooks/` directory.

## Experiments & Implementations

The repository is organized around practical experiments rather than a fixed model limitation.

| Experiment | Description | Status |
|---|---|---|
| Image Object Detection | Detect objects in static images | In Progress |
| Image Face Detection | Detect human faces in images | In Progress |
| Combined Detection | Combine object and face detection outputs | In Progress |
| Webcam Detection | Perform real-time detection using webcam streams | In Progress |
| CPU Inference | Run detection models using CPU | Planned |
| GPU Inference | Explore CUDA-based inference | Planned |
| Model Comparison | Experiment with different model variants | Planned |
| Performance Analysis | Explore inference time and FPS | Planned |

## Results & Visualizations

Detection outputs, screenshots, and other visual results will be stored in:

```text
assets/
├── screenshots/
├── demo-images/
└── videos/
```

Actual experiment results will be added as the project develops.

## Learning Outcomes

Through this project, I aim to develop practical knowledge of:

- Computer Vision fundamentals.
- Object detection and face detection.
- Pretrained deep learning models.
- YOLO model inference.
- Image processing with OpenCV.
- Real-time video processing.
- Bounding boxes and confidence scores.
- Integration of multiple detection models.
- CPU and GPU inference.
- Practical experimentation and model evaluation.

## Future Improvements

Potential areas of exploration include:

- Experimenting with different YOLO architectures and model variants.
- Adjustable confidence thresholds.
- Object tracking and detection.
- Video file processing.
- Detection performance benchmarking.
- FPS measurement and inference optimization.
- Custom object detection.
- Additional computer vision applications.
- A graphical user interface for easier interaction.

## References & Acknowledgements

This project uses open-source tools, libraries, and pretrained models.

- [Ultralytics](https://github.com/ultralytics/ultralytics)
- [YOLO Face — akanametov](https://github.com/akanametov/yolo-face)
- [OpenCV](https://github.com/opencv/opencv)
- [PyTorch](https://github.com/pytorch/pytorch)

Thanks to the developers and open-source communities behind these projects for making their tools and research accessible.

Please refer to the respective repositories for their licenses and usage conditions.

## Author

**Gursimran Singh**

- GitHub: [@gursimranai](https://github.com/gursimranai)

---

<p align="center">
  <i>Learning, experimenting, and building practical Computer Vision applications.</i>
</p>