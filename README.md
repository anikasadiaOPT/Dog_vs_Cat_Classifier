# Dog vs Cat Classifier

This repository contains a Convolutional Neural Network (CNN) model for classifying images as either dogs or cats. The project is built using Python, TensorFlow, and Keras, and leverages the Kaggle dataset for dogs and cats.

## Table of Contents

- [Overview](#overview)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [Directory Structure](#directory-structure)
- [Acknowledgements](#acknowledgements)

## Overview

The main goal of this project is to train a CNN on the Kaggle Dogs vs Cats dataset and evaluate its performance on test images. You can find all relevant code and notebooks for building, training, and testing the model in this repository.

## Setup Instructions

Follow the steps below to get started:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/anikasadiaOPT/Dog_vs_Cat_Classifier.git
   cd Dog_vs_Cat_Classifier
   ```

2. **Install the required packages:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Generate your Kaggle API token:**
   - Go to your Kaggle account (> [Kaggle API Docs](https://www.kaggle.com/docs/api)).
   - Select "Account" and click "Create New API Token."
   - This downloads `kaggle.json`.
   - Move `kaggle.json` to `~/.kaggle/kaggle.json`:
     ```bash
     mkdir -p ~/.kaggle
     mv /path/to/kaggle.json ~/.kaggle/
     chmod 600 ~/.kaggle/kaggle.json
     ```

4. **Download the Dogs vs Cats dataset:**
   ```bash
   kaggle competitions download -c dogs-vs-cats
   unzip dogs-vs-cats.zip -d data/
   ```

5. **Run the CNN notebook:**
   Open `cnn.ipynb` in Jupyter Notebook or Colab, and run all cells to train and evaluate the dog-vs-cat model.

   ```bash
   jupyter notebook cnn.ipynb
   ```

6. **Model outputs and predictions:**  
   After running the notebook, predictions and evaluations will be saved to the specified output folders.

## Usage

- **Training:**  
  The `cnn.ipynb` notebook covers data loading, preprocessing, model architecture, training, and evaluation.
- **Testing:**  
  You can test the model by putting new images into the test directory specified in the notebook and running inference cells.

## Directory Structure

```
Dog_vs_Cat_Classifier/
│
├── cnn.ipynb                # Main notebook for model training and evaluation
├── README.md                # Project instructions
├── requirements.txt         # Python dependencies
├── data/                    # Contains the dataset (after unzip)
│   ├── train/
│   ├── test/
│   └── ... 
└── model/                   # Saved models
```

## Acknowledgements

- [Kaggle Dogs vs Cats Competition](https://www.kaggle.com/c/dogs-vs-cats)
- TensorFlow & Keras documentation

---

**If you have questions, please create an issue in this repository.**
