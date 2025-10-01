Olivetti Faces Recognition
<u>Project Overview</u>

The Olivetti Faces Recognition project implements a machine learning system to classify grayscale face images into 40 individuals using the Olivetti Faces dataset.

This project demonstrates a complete ML workflow, including data exploration, visualization, training, and evaluation, making it ideal for beginners and portfolio presentation.

<u>Objective</u>

Predict the individual in a face image (from 40 people).

Explore and visualize image data to connect raw pixels to actual faces.

Build a reproducible pipeline for image classification.

<u>Dataset Details</u>

Name: Olivetti Faces Dataset

Source: scikit-learn (sklearn.datasets.fetch_olivetti_faces)

Total Images: 400

Number of Classes (Individuals): 40

Images per Person: 10

Image Size: 64 × 64 pixels, grayscale

Pixel Values: Normalized between 0 and 1

Target Values: Labels from 0–39 representing each individual

<u>Project Workflow</u>
1. Load and Explore Dataset

Load dataset using fetch_olivetti_faces().

Inspect shapes:

data → (400, 4096)

images → (400, 64, 64)

target → (400,)

Examine target labels to verify class distribution.

2. Visualize Sample Faces

Display images with target labels.

Example of Person ID 0:

(Replace the path with your actual image in the repo)

3. Split Data

Split dataset into training (80%) and testing (20%) sets.

Use stratified split to maintain class balance.

4. Train Classifier

K-Nearest Neighbors (KNN) used as baseline.

Model learns pixel patterns to classify individuals.

5. Evaluate Model

Predict on test images and compute accuracy (~88.75% achieved).

Generate a confusion matrix to visualize misclassifications:

(Replace the path with your actual image in the repo)

6. Optional Improvements

Apply PCA / eigenfaces for dimensionality reduction.

Try SVM, Logistic Regression, or Neural Networks.

Hyperparameter tuning and data augmentation.

<u>Technologies Used</u>

Python 3.x – programming language

scikit-learn – dataset handling, model training, evaluation

NumPy – numerical operations

Pandas – data exploration

Matplotlib / Seaborn – visualization

<u>Key Learning Outcomes</u>

Understand image dataset structure and targets.

Visualize and interpret pixel data as actual faces.

Implement a complete ML pipeline for classification.

Evaluate models using accuracy and confusion matrices.

Gain a foundation for more advanced face recognition techniques.
