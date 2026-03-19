# SafetyEye - AI-Powered Workplace Safety Monitor

An AI-powered real-time workplace safety monitoring system that automatically 
detects PPE (Personal Protective Equipment) violations on construction sites 
using YOLOv8 computer vision.

---

## Project Overview

SafetyEye uses a trained YOLOv8 model to detect workers and identify safety 
violations such as missing helmets, safety vests and masks from live video 
feeds or recorded footage.

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3.11.9 | Core programming language |
| YOLOv8 (Ultralytics) | Object detection model |
| OpenCV | Video capture and visualization |
| PyTorch | Deep learning framework |
| Google Colab | GPU training environment |
| Streamlit | Dashboard (Milestone 4) |
| SQLite | Violation logging (Milestone 4) |

---

## Dataset

- Source: Roboflow Construction Site Safety Dataset
- Total Images: ~3000 labeled images
- Classes: 10 (Hardhat, Mask, NO-Hardhat, NO-Mask, NO-Safety Vest, 
  Person, Safety Cone, Safety Vest, Machinery, Vehicle)
- Split: 70% Train / 20% Validation / 10% Test

---

## Model Performance

### Validation Results
| Metric | Score |
|---|---|
| Precision | 89.1% |
| Recall | 68.8% |
| mAP50 | 78.3% |

### Test Results (Official)
| Metric | Score |
|---|---|
| Precision | 85.5% |
| Recall | 66.7% |
| mAP50 | 73.3% |

---

## Project Structure
```
SafetyEye/
├── dataset/
│   ├── train/
│   ├── valid/
│   └── test/
├── models/
│   └── best.pt
├── src/
│   ├── data_prep.py
│   ├── train.py
│   └── detect.py (Milestone 3)
├── reports/
│   ├── Milestone1_Report.docx
│   └── Milestone2_Report.docx
├── dataset.yaml
└── requirements.txt
```

---

## Milestones

| Milestone | Description | Status |
|---|---|---|
| 1 | Data Preparation and Environment Setup | Complete |
| 2 | Model Training and PPE Detection | Complete |
| 3 | Real-Time Detection and Alert System | In Progress |
| 4 | Dashboard and Reporting | Upcoming |

---

## Reports

- Milestone 1 Report - reports/Milestone1_Report.docx
- Milestone 2 Report - reports/Milestone2_Report.docx

---

## How to Run
```bash
# Clone the repository
git clone https://github.com/preethiguggulla/SafetyEye.git

# Install dependencies
pip install -r requirements.txt

# Run detection (Milestone 3)
python src/detect.py
```

---

## Author

Preethi Guggulla
