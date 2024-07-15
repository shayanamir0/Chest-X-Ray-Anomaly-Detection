# Chest X-Ray Anomaly Detection using Autoencoder

This project focuses on detecting lung diseases from chest X-ray images using an autoencoder architecture for anomaly detection. The dataset used is the [Japanese Society of Radiological Technology (JSRT) Database](http://db.jsrt.or.jp/eng.php).

## Table of Contents
- [Introduction](#introduction)
- [Model Architecture](#model-architecture)
- [Training and Results](#training-and-results)

## Introduction
Lung diseases such as pneumonia and lung cancer can be life-threatening if not detected early. This project aims to leverage an autoencoder model to automatically detect anomalies in chest X-ray images that may indicate the presence of lung diseases, thereby aiding in early diagnosis and treatment.

## Model Architecture
The project employs a simple autoencoder architecture for anomaly detection. Below is an overview of the model architecture:

![Model Architecture]([![JSRT Autoenc model](https://github.com/user-attachments/assets/3bc6912b-f344-4ce3-99c4-b9cdcaf4ffc1)])

The autoencoder model consists of an encoder that compresses the input image into a lower-dimensional representation and a decoder that reconstructs the image from this representation. Anomalies are detected based on the reconstruction error, with higher errors indicating potential anomalies.

## Training and Results
The model was trained on the JSRT dataset using 256*256 images with appropriate data preprocessing techniques. The following metric was used to evaluate the model performance:

- **Reconstruction Error**: Measures the difference between the original and reconstructed images. Higher errors indicate potential anomalies.

### Results
After training the model, a sapmle prediction has been done which detects 3 anomalies.
