# Capsule-Enhanced Feature Extraction with Attention Mechanism (CEFEAM)

## Description
This repository provides the Python implementation of the proposed
Capsule-Enhanced Feature Extraction with Attention Mechanism (CEFEAM) model
for robust Acute Lymphoblastic Leukemia (ALL) diagnosis from peripheral blood
smear images. The implementation is designed to reproduce the experimental
results reported in the corresponding research article under limited data
conditions.

## Dataset Information
- Dataset: ALL-IDB (Acute Lymphoblastic Leukemia Image Database)
- Source: Publicly available dataset
- Image type: Peripheral blood smear microscopic images
- Tasks:
  - Binary classification (ALL vs. Normal)
  - Multi-class classification (ALL, other leukemia types, Normal)
- Data splitting: 6-fold cross-validation

## Code Information
- Programming Language: Python
- Deep Learning Framework: TensorFlow / Keras
- Main file: main.ipynb
- Backbone Network: DenseNet-201 (pretrained)
- Additional Modules:
  - Attention Mechanism for region-focused feature enhancement
  - Capsule Network layers for preserving spatial hierarchies

## Methodology
1. Image loading and preprocessing
2. Feature extraction using DenseNet-201
3. Attention-based feature refinement
4. Capsule network integration for spatial relationship modeling
5. Classification using fully connected capsule outputs
6. Model evaluation using k-fold cross-validation

## Usage Instructions
1. Install required dependencies:
   pip install -r requirements.txt
2. Open the Jupyter notebook:
   main.ipynb
3. Run the cells sequentially to train and evaluate the model.

## Requirements
- Python >= 3.8
- TensorFlow
- NumPy
- OpenCV
- Scikit-learn
- Matplotlib
- tqdm

## Evaluation Metrics
- Accuracy
- Recall
- Precision
- F1-score
- Confusion Matrix

## Experimental Results
- Binary classification accuracy: 99.2%
- Binary classification recall: 99.25%
- Multi-class classification accuracy: 97.18%
- Multi-class classification recall: 96.49%

## Notes
- The experiments are conducted using 6-fold cross-validation.
- The model is designed for scenarios with limited training data.

## Citations
If you use this code, please cite the corresponding research article:
"Capsule-Enhanced Feature Extraction with Attention Mechanism for Robust Acute
Lymphoblastic Leukemia Diagnosis from Limited Blood Smear Data"

## License
This repository is intended for academic and research purposes only.
