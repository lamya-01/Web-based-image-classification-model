# Web-based-image-classification-model

## Overview

This project demonstrates how to use Teachable Machine and TensorFlow.js to create a web-based image classification model. The model is trained to classify images into three categories: Apple, Orange, and Other Fruits/Vegetables. The classification is performed in real-time using your webcam.

## Dataset

- Apple and Orange Dataset: The dataset for Apple and Orange images is obtained from Kaggle. You can access it [here](https://www.kaggle.com/datasets/balraj98/apple2orange-dataset).
  
- Other Fruits and Vegetables Dataset: The dataset for the "Other" category, which includes a variety of fruits and vegetables, is also sourced from Kaggle. You can access it [here](https://www.kaggle.com/datasets/kritikseth/fruit-and-vegetable-image-recognition).

## Project Files

- index.html: The HTML file that creates the structure for the webpage. It includes buttons to start the webcam and containers to display the webcam feed and the classification results.
  
- Teachable Machine Model: The trained image classification model is created using Teachable Machine. The model is exported and saved in the my_model directory, which contains:
  - model.json: The model architecture and weights.
  - metadata.json: Metadata about the model such as labels.
  - weights.bin: The binary weights file used by the model.

- JavaScript: The JavaScript code included in index.html loads the model, initializes the webcam, and performs real-time predictions. The predictions are displayed as text below the webcam feed.

## How to Use

1. Model Setup:
    - Ensure that the my_model directory is in the same directory as index.html. The my_model directory should include the model.json, metadata.json, and weights.bin files.

2. Running the Model:
    - Open index.html in your browser.
    - Click the Start button to initialize the webcam and load the model.
    - The webcam feed will appear on the webpage, and the model will start predicting in real-time.
    - The classification results will be displayed below the webcam feed, showing the predicted class and its confidence level.

3. Webcam Setup:
    - The webcam is set to flip the image horizontally (mirroring). You can change this by modifying the flip variable in the JavaScript code.

4. Prediction Loop:
    - The loop function continuously updates the webcam frame and performs predictions.
    - The predict function runs the model on the current webcam image and updates the labels with the class name and probability.

## Requirements

- A modern web browser that supports WebRTC for webcam access.
- A stable internet connection to load TensorFlow.js and the Teachable Machine model.
- A webcam or a built-in camera on your device.

## Notes

- The model accuracy may vary based on the quality of the dataset and the training process in Teachable Machine.
- The webcam feed is set to 200x200 pixels. You can adjust the width and height in the JavaScript code if needed.

## Acknowledgments

- The datasets used in this project were sourced from Kaggle.
- This project uses Teachable Machine, a tool developed by Google Creative Lab, and TensorFlow.js.

## Example
![لقطة شاشة 2024-08-12 115647](https://github.com/user-attachments/assets/754699b2-ee23-47ec-9999-73c82709f840)

