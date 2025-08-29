# pneumonia-xray-classifier
A deep learning pipeline for pneumonia detection using chest X-ray images. Includes custom CNN development, model evaluation, Grad-CAM interpretability, and an interactive ML app for real-time prediction.

## 🔍 Project Overview

- Binary classification of chest X-ray images: **Normal** vs **Pneumonia**
- Custom CNN architecture trained and evaluated on a labeled dataset
- Comparison with a pre-trained MONAI DenseNet121 model
- Grad-CAM visualizations for model interpretability
- Interactive ML app for image upload and prediction

## 🧠 Model Highlights

- **Custom CNN** trained with weighted cross-entropy loss to handle class imbalance
- **Evaluation metrics**: Accuracy, Precision, Recall, F1-score, ROC AUC
- **Final model selected** based on balanced performance across metrics
- **Grad-CAM** used to visualize model attention on lung regions

## 📁 Repository Structure
```
├── Pneumonia_Xray_Classifier.ipynb # Main notebook with full pipeline
├── final_pneumonia_model_full.pth # Saved final model object (Custom CNN)
└── README.md # Project overview
```

## 📦 Dataset

This project uses the [Chest X-ray Pneumonia dataset](https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia/data) by Paul Timothy Mooney, available on Kaggle.  
To use the notebook, download and extract the dataset into the `data/` directory following the original folder structure (`train/`, `val/`, `test/`).

## 🚀 How to Use

1. Clone the repo and open the notebook in Google Colab
2. Download the dataset from Kaggle and place it in the `data/` folder
3. Upload your own chest X-ray image or use a sample from the dataset
4. Run the prediction and view the Grad-CAM visualization
5. Modify thresholds or model architecture as needed

## 📜 License

This project is for educational and research purposes. No clinical use intended.
