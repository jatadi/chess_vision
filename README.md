# Chess Vision: Enhancing Chess Piece Recognition Using Deep Learning

## Introduction
Chess Vision is a project focused on applying deep learning to enhance chess piece recognition. Our approach addresses the challenge of accurately identifying different chess pieces, which is crucial for game analysis and digitization.

## Motivation
Our goal is to bridge the gap between physical chess gameplay and digital analysis tools, aiding in automated game logging, real-time move tracking, and interactive training programs.

## Dataset Composition
We used a balanced dataset of six types of chess pieces (Knights, Bishops, Rooks, Queens, Kings, and Pawns) with each class having around 110 images. The images were preprocessed to a uniform size of 224x224 pixels.

## Preprocessing and Data Augmentation
- **Resizing**: Standardizing images to 224x224 pixels.
- **Normalization**: Scaling pixel values to a 0-1 range.
- **Augmentation Techniques**: Including rotation, width and height shifts, shear transformation, zoom, and horizontal flip.

## Methodology
- **Initial Multiclass Model**: We started with a multiclass classification approach using a CNN.
- **Transition to Binary Classification Models**: To improve accuracy, we shifted to developing individual binary models for each chess piece, based on the VGG16 architecture.
- **Combining Binary Models**: Using a weighted voting system, the outputs of the six binary models were combined to improve overall performance.
- **Generative Adversarial Networks (GANs)**: Employed for generating synthetic images of chess pieces, enhancing training data diversity.

## Results and Evaluation
- **Binary Model Evaluations**: We assessed each model using metrics like accuracy, precision, recall, F1-score, and ROC-AUC curves.
- **Combined Model Performance**: Demonstrated effective use of the weighted voting system for accurate predictions.
- **Impact of GANs**: GANs contributed to dataset enhancement and model robustness, though integration posed challenges.

## Conclusion
The project was a successfull comparative analysis of predictive models in chess piece recognition. Future work will focus on refining these models for enhanced performance and accuracy.

## Installation Instructions

### Prerequisites
- Python 3.x
- Jupyter Notebook or JupyterLab
- Access to the internet to download the dataset from Google Drive

### Steps
1. **Clone the Repository:**
   ```bash
   git clone https://github.com/jatadi/chess_vision.git
   cd Models

**Download the Dataset:**

    Link to the dataset: https://www.kaggle.com/datasets/niteshfre/chessman-image-dataset

**Usage Instructions:**

    Open the Jupyter Notebook:
        After launching Jupyter Notebook or JupyterLab, navigate to the directory containing the cloned repository.
        Open the .ipynb files in the order they are meant to be executed, if there's a specific order.

    Run the Notebooks:
        Execute the cells in each notebook. Make sure to read any comments or documentation within the notebooks to understand the flow.

