# breastcancerpred
Streamlit App - [https://breastcancerpred1.streamlit.app/]. 

LinkedIn - Danush Rajaram[https://www.linkedin.com/in/danushrajaram/]. 

Breast Cancer Predictor

Overview

The Breast Cancer Predictor is a machine learning-based web application designed to assist medical professionals in predicting whether a breast mass is benign or malignant. It uses cytology lab data and measurements of cell nuclei characteristics to make predictions using a logistic regression model. The app also provides a radar chart visualization for an intuitive representation of the input features.

This tool should serve as an aid to medical professionals and not as a standalone diagnostic system.

Features

Machine Learning Model: Trained logistic regression model to classify breast masses.

Interactive Sidebar: Input sliders for updating measurements manually.

Radar Chart Visualization: Comparison of mean, standard error, and worst-case values for various cell nucleus measurements.

Prediction Details:

Indicates whether the mass is benign or malignant.

Displays probabilities for both outcomes.

Requirements

Python Libraries

Ensure the following Python libraries are installed:

pandas

scikit-learn

streamlit

numpy

plotly

Install the required libraries using pip:

pip install pandas scikit-learn streamlit numpy plotly

Dataset

The application uses a dataset named data.csv. Ensure this file is placed in the same directory as the application files. The dataset should contain the following:

Columns for various cell measurements (e.g., radius_mean, texture_mean, etc.).

A diagnosis column indicating if the mass is malignant (M) or benign (B).

No missing or extraneous columns (e.g., Unnamed: 32, id).

Setup and Execution

Step 1: Training the Model

Run the following command to train the model and generate the required pickle files (model.pkl and scaler.pkl):

python main.py

This will:

Preprocess the dataset.

Train the logistic regression model.

Save the trained model and scaler for later use.

Step 2: Running the Application

Launch the Streamlit web application using:

streamlit run app.py

This will open the application in your default web browser.

Step 3: Interacting with the App

Use the sidebar sliders to adjust the input measurements manually.

Observe the radar chart for visual insights into the provided data.

View predictions and probabilities for benign and malignant classifications in the main panel.

Application Files

main.py: Script to train the model and save it for deployment.

app.py: Streamlit-based application for interactive predictions.

data.csv: Input dataset containing breast cancer data.

style.css: CSS file to style the application.

Notes

The application requires the model.pkl and scaler.pkl files to function. Ensure these files are present in the working directory before running app.py.

Use this tool as a supplement to professional diagnostic methods and not as a replacement.

Example Usage

Training the Model:

python main.py

Starting the Web App:

streamlit run app.py

Input Adjustments:

Adjust measurements via the sliders on the sidebar.

Visualize changes in the radar chart and observe predictions.
