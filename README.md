Part 2: Computer Vision for Manufacturing Defect Detection
Project Overview
This project focuses on building a Computer Vision prototype to automate quality inspection in a manufacturing setting. The goal is to classify product images into four categories: Normal, Scratch, Dent, and Stain using a neural network.

Task 1: Problem Identification
The dataset represents an Image Classification problem.

Reason: We are categorizing the entire image into a single discrete class based on the visual features present. This is appropriate because the goal is to identify the type of defect rather than locating its exact coordinates or boundaries.

Task 6: CNN Concept Explanation
Convolution: This is a mathematical operation that uses "filters" to scan an image. It helps the model detect important visual features like edges, textures, and specific shapes of defects.

Pooling: Pooling layers (like Max Pooling) reduce the spatial size of the image. This keeps only the most important information, making the model faster and less likely to overfit.

ReLU (Rectified Linear Unit): This activation function replaces negative pixel values with zero. It helps the network learn non-linear patterns, which is essential for understanding complex images.

CNN vs. Regular Networks: Regular feed-forward networks treat images as a flat list of pixels, losing the "spatial" context. CNNs are superior because they preserve the relationship between neighboring pixels, allowing the model to "see" shapes and patterns.

Task 7: Business Use Case Mapping
Domain: Manufacturing
This solution can be implemented in a Smart Factory environment. High-speed cameras on a production line can capture images of products, and this CNN model can automatically flag items with scratches or dents. This reduces the need for manual human inspection, speeds up the production process, and ensures that only defect-free products reach the customers.

Model Performance Summary
Based on the experiments conducted in the notebook:

Primary Model: MLP/CNN Prototype.

Accuracy: The model successfully learned to distinguish between the four defect classes, as shown in the Confusion Matrix.

Repository Structure
notebook.ipynb: Complete code for data loading, preprocessing, and model training.

requirements.txt: List of dependencies (OpenCV, Scikit-learn, etc.).

results/: Contains accuracy_loss_curves.png and confusion_matrix.png.

sample_predictions/: Contains prediction_outputs.png showing the model's predictions on test images.