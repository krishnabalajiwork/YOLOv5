# YOLOv5 Object Detection for Indian Languages and Numerals

This repository contains a YOLOv5 model for detecting text in various Indian languages and numerals in images.

---

## 📝 Description

This project uses the YOLOv5 object detection algorithm to identify and locate text from the following classes:
* Bengali
* English
* Gujarati
* Hindi 
* Kannada
* Malayalam
* Numeral
* Punjabi
* Tamil
* Telugu

Due to file size limitations on GitHub, the `YOLOv5.ipynb` notebook could not be uploaded directly. You can access the notebook and the required dataset from the Google Drive link below.

---

## 📁 Project Files

* **YOLOv5.ipynb**: The main Jupyter notebook for training and running the object detection model.
* **data.yaml**: The configuration file for the dataset. You will need to edit this file to point to the dataset location in your Google Drive.
* **outputs/**: A directory containing sample output images from the trained model.

---

## 🚀 Getting Started

### Prerequisites

* A Google account to access Google Colab and Google Drive.

### Setup Instructions

1.  **Download the project files:**
    * Download the `YOLOv5.ipynb` notebook and the dataset from this Google Drive link: [https://drive.google.com/drive/u/0/folders/1Drcek-L7-444xoFM6pvqV9u1uJ2pikqY](https://drive.google.com/drive/u/0/folders/1Drcek-L7-444xoFM6pvqV9u1uJ2pikqY)
    * Upload the notebook and the dataset to your Google Drive.

2.  **Configure `data.yaml`:**
    * Open the `data.yaml` file.
    * You need to specify the paths to your training and validation data, the number of classes, and the class names. Here is a template to guide you:

    ```yaml
    train: ../yolo_formatted_dataset/images/train
    val: ../yolo_formatted_dataset/images/val

    nc: 10

    names: ['Bengali', 'English', 'Gujarati', 'Hindi', 'Kannada', 'Malayalam', 'Numeral', 'Punjabi', 'Tamil', 'Telugu']
    ```

    Make sure the `train` and `val` paths point to the correct locations of your dataset in your Google Drive.

---

## 💻 How to Run

1.  Open the `YOLOv5.ipynb` notebook in Google Colab.
2.  Follow the steps in the notebook:
    * **Mount Google Drive**: This will give the notebook access to the files you uploaded.
    * **Install Dependencies**: The notebook will install the necessary libraries, including `ultralytics`.
    * **Train the Model**: Run the training cell to train the YOLOv5 model on the dataset. The notebook is set to train for 20 epochs, but you can adjust this.
    * **Run Inference**: After training, you can upload an image to the notebook to see the model's predictions.
<img width="288" height="583" alt="image" src="https://github.com/user-attachments/assets/a09ebbc5-1beb-4311-a111-4ec3f7acc87a" />

---
