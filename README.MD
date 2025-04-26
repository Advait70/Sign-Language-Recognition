# AI-Powered Sign Language Recognition System

This project aims to recognize American Sign Language (ASL) alphabets using deep learning. A Convolutional Neural Network (CNN) based model, utilizing MobileNet architecture, has been trained to classify static hand gesture images.

The project demonstrates how pre-trained models can be used for fast and accurate predictions without retraining.

---

## Project Description

- The model is trained on the ASL Alphabet Dataset to recognize letters A-Z, along with DEL, SPACE, and NOTHING gestures.
- A `Hand_Signs/` folder is included, containing sample gesture images for easy understanding of the signs.
- The project is divided into two key notebooks:
  - `s1.ipynb`: Full code including data preprocessing, model training, evaluation, and saving the model. Viewable directly on GitHub.
  - `output.ipynb`: Lightweight demo notebook that loads the pre-trained model and makes a sample prediction. Intended for quick testing without retraining.

---

## Repository Structure

- `s1.ipynb` - Full model training and evaluation notebook (viewable on GitHub).
- `output.ipynb` - Quick demo notebook for instant model prediction.
- `sign_language_model_mobilenet.h5` - Saved MobileNet model.
- `sign_language_model.h5` - Backup saved model.
- `Hand_Signs/` - Reference images showing gestures for each letter/sign.
- `README.md` - Project documentation.

---

## How to Run the Project

1. Clone or download this repository.
2. (Optional) Download the full ASL Alphabet Dataset if you wish to retrain the model (link below).
3. Open `output.ipynb` using Jupyter Notebook or Google Colab.
4. Run all cells to load the pre-trained model and predict a hand sign.

No retraining is required for using the demo notebook.

---

## Dataset

The ASL Alphabet dataset is not included in this repository due to its large size (~1 GB).

You can download it from the following link:
- [Download ASL Alphabet Dataset](https://storage.googleapis.com/kaggle-data-sets/23079/29550/bundle/archive.zip?...)

After downloading, extract the dataset and organize it appropriately if you plan to retrain the model using `s1.ipynb`.

---

## Requirements

Install the following libraries:

```bash
pip install tensorflow numpy opencv-python matplotlib