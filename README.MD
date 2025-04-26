# AI-Powered Sign Language Recognition System

This project is designed to recognize American Sign Language (ASL) alphabets using deep learning. A Convolutional Neural Network (CNN) based model, specifically utilizing MobileNet architecture, has been trained on the ASL Alphabet Dataset to classify hand gestures representing different letters.

The objective of this project is to provide a fast and accurate prediction of sign language gestures without needing to retrain the model each time.

---

## Project Description

- This project involves building a model that can classify static images of hand gestures corresponding to ASL alphabets.
- The model was trained on the ASL Alphabet Dataset and optimized using MobileNet for better efficiency.
- The project has been divided into two parts:
  - **s1.html**: Contains the full code from data import, preprocessing, model training, evaluation, and saving of the model. It shows the complete training pipeline and outputs. This file is for reference and should be viewed for understanding the full model development process. It is not meant for execution.
  - **output.ipynb**: A lightweight notebook designed to quickly load the pre-trained model and make a prediction. Recruiters or reviewers can simply run this notebook without retraining the model to instantly view a prediction result.

Additionally, a folder named **Hand_Signs** has been included, which contains reference images for the ASL gestures from A-Z, along with DEL, SPACE, and NOTHING. This is intended to help recruiters or users understand the gestures the model is trained to recognize.

---

## Repository Structure

- `s1.html` - Full training and evaluation code, model building process, and outputs (for reading only).
- `output.ipynb` - Quick demo notebook that loads the saved model and predicts sign language letters (runnable).
- `sign_language_model_mobilenet.h5` - Saved MobileNet model trained on ASL Alphabet Dataset.
- `sign_language_model.h5` - Backup saved model.
- `Hand_Signs/` - Contains images of all sign gestures (A-Z, Del, Space, Nothing) for visual reference.
- `README.md` - Project documentation and instructions.

---

## How to Run the Project

1. Clone or download this repository.
2. Download the full ASL Alphabet dataset from the link provided below if you wish to retrain the model. (Retraining is optional and not necessary for demo.)
3. Place the dataset appropriately if retraining is needed.
4. Open `output.ipynb` using Jupyter Notebook or Google Colab.
5. Run all cells to load the pre-trained model and perform a prediction on sample input.

Note: For demo purposes, no retraining is required. The pre-trained model will be used directly.

---

## Dataset

The ASL Alphabet training dataset is not included in this repository due to its large size (~1 GB).

You can download the dataset from the following link:
- [Download ASL Alphabet Dataset](https://storage.googleapis.com/kaggle-data-sets/23079/29550/bundle/archive.zip?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=gcp-kaggle-com%40kaggle-161607.iam.gserviceaccount.com%2F20250307%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20250307T123700Z&X-Goog-Expires=259200&X-Goog-SignedHeaders=host&X-Goog-Signature=3f887cf8868bcc49c58ccaafe0ec99bad6ad969a2878368c9308c15c1bf5ec6d8319f5315a7eb9d9b021ff34c570d0356163f37db4f7fd4de70770eb3b3c836440de2d65d39d53414f1b483ac9f2ea2d3933500a44c1ab86cee25a94f68c0a02f52312ac35acf4e85f1729c63220fd7f9a30e897f3f3014eb545f80b386bfc4c08d279d973ed6ccdb254df5e4348d825bce6126acd94337af422f5c6951f43b4663b47aec4e9258bebc3616cc1c2235eb5487d5a167d2859622f86118c332ea325cfa35cc0be0f122c4e8c82f3a60c8d7727900e1c6285a769a139de0b5e94fddb18506dbda8c91f3a31e8ce959ae5c1a9221443f5d8d60393c419a202884034)

After downloading:
- Extract the dataset and organize it properly if you plan to retrain the model using `s1.html`.

---

## Requirements

Install the following libraries to run this project:

- Python 3.7 or above
- TensorFlow
- NumPy
- OpenCV
- Matplotlib

To install all required libraries:

```bash
pip install tensorflow numpy opencv-python matplotlib