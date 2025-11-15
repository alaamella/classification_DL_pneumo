# Automated Diagnosis of Pneumonia from Chest X-Ray Images using EfficientNet 🏥📸

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![TensorFlow](https://img.shields.io/badge/TensorFlow-2.x-orange.svg)
![Deep Learning](https://img.shields.io/badge/Deep%20Learning-EfficientNet-green.svg)

This project utilizes the EfficientNet model for automated diagnosis of pneumonia from chest X-ray images. It is a fine-tuned version of the pre-trained EfficientNet model adapted for binary classification to differentiate between normal and pneumonia cases.

## Features 🌟
- Utilizes the EfficientNet model, known for its efficiency and accuracy in image classification.
- Implements image data augmentation to enhance model generalization.
- Includes detailed preprocessing steps for dataset preparation.
- Provides performance evaluation metrics such as accuracy, precision, recall, F1-score, and AUC.

## Setup and Installation 🛠️
1. Clone the repository.
2. Install TensorFlow and other required libraries listed in `requirements.txt`.
3. Prepare the dataset, following the preprocessing steps outlined in the code.

## Repository Structure 📂

```
classification_DL_pneumo/
├── data/
│   └── chest_xray/
│       ├── train/
│       │   ├── NORMAL/
│       │   └── PNEUMONIA/
│       ├── val/
│       │   ├── NORMAL/
│       │   └── PNEUMONIA/
│       └── test/
│           ├── NORMAL/
│           └── PNEUMONIA/
├── PLGaultier/
│   └── model.ipynb (PyTorch/FastAI)
├── MJAHMADEE/
│   ├── MainCode_Approach1.ipynb
│   ├── MainCode_Approach2.ipynb
│   ├── MainCode_Approach1.py
│   └── MainCode_Approach2.py
├── bhavya1600/
│   └── Chest_Pneumonia_Classification.ipynb
└── nikoneri/
    └── CHEST_X-RAY_PNEUMONIA_CLASSIFICATION.ipynb
```

Each contributor-specific folder holds their respective notebooks and scripts. The `data` directory is pre-populated with the folder structure expected by the notebooks; populate the `train`, `val`, and `test` splits before running experiments.

### Contributor Notebooks

- **PLGaultier/model.ipynb** – A FastAI implementation that fine-tunes a ResNet-34 backbone and exports the trained learner for reuse.
- **bhavya1600/Chest_Pneumonia_Classification.ipynb** – A TensorFlow/Keras workflow with custom CNN architecture, data augmentation, and confusion-matrix reporting.
- **nikoneri/CHEST-X-RAY_PNEUMONIA_CLASSIFICATION.ipynb** – An EfficientNetB3 transfer-learning pipeline with staged fine-tuning and test-set evaluation.

## Data 📁
The project uses chest X-ray images from publicly available datasets. These images are processed and labeled into two classes: NORMAL and PNEUMONIA.

## Model Training and Evaluation 🚀
- Train the model using the preprocessed dataset with image augmentation to improve robustness.
- Evaluate the model using accuracy, precision, recall, F1-score, and ROC-AUC metrics.
- Visualize results with confusion matrices, precision-recall curves, and ROC curves.

## Contributing 🤝
Contributions to improve the model and its implementation are welcome. Please fork the repository, make your changes, and submit a pull request.

## License 📜
The project is licensed under the MIT License - see the LICENSE file for more details.

## Acknowledgements 🙌
- Creators of the EfficientNet model for their contributions to the field of deep learning.
- Publicly available chest X-ray datasets that facilitate medical imaging research.

For more information and to view the source code, visit the [GitHub repository](https://github.com/MJAHMADEE/Automated_Diagnosis_of_Pneumonia_from_Classification_of-Chest_XRay_Images_using_EfficientNet/).
