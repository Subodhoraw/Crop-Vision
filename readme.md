# 🌿 CropVision — Plant Disease Detection

**Infotact DS/ML Internship | Project 2: Agriculture & Smart Farming**

A deep learning Computer Vision system that detects plant diseases from leaf images using CNNs and Transfer Learning (ResNet50/MobileNet), trained on the PlantVillage dataset.

---

## 📁 Project Structure

```
cropvision/
├── data/
│   └── PlantVillage/          # Raw dataset (gitignored)
├── outputs/                   # EDA plots, model outputs
├── notebooks/                 # Jupyter notebooks
├── week1_eda.py               # EDA + class distribution
├── week1_preprocessing.py     # Preprocessing + augmentation + splits
├── requirements.txt
├── .gitignore
└── README.md
```

## 🗓️ 4-Week Roadmap

| Week | Focus | Status |
|------|-------|--------|
| 1 | EDA, Preprocessing, Augmentation, Splits | 🔄 In Progress |
| 2 | Custom CNN Architecture + Baseline Training | ⏳ Upcoming |
| 3 | Transfer Learning (ResNet50) + Hyperparameter Tuning | ⏳ Upcoming |
| 4 | Evaluation, Inference Script, Deployment | ⏳ Upcoming |

## 🚀 Setup

```bash
# Clone repo
git clone https://github.com/subodhoraw/cropvision.git
cd cropvision

# Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Download dataset
kaggle datasets download -d emmarex/plantdisease
unzip plantdisease.zip -d data/PlantVillage
```

## 🎯 Target KPIs

- **Accuracy**: > 90% on test set
- **Recall**: Maximized (missing diseased leaf = false negative = crop spread)
- **Input size**: 224×224 RGB

## 📊 Dataset

**PlantVillage** — 50,000+ labeled leaf images across 38 plant disease classes  
Source: [Kaggle](https://www.kaggle.com/datasets/emmarex/plantdisease)

## ⚠️ Important

- Raw dataset (`data/`) is gitignored — do NOT commit raw images
- Model weights (`.h5`, `.pkl`) are gitignored
- API keys must be set as environment variables — never hardcode
- **Commit 3–5 times per day** — monolithic final push = disqualification
