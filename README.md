# Hermes Haven: Fall Detection and Response System for Elderly Care

Hermes Haven is a project developed to detect and respond to falls among the elderly using kinematic data collected from OpenCap sensors. It employs machine learning techniques, specifically a linear Support Vector Machine (SVM) model and a threshold-based classifier, to predict and identify sustained falls. Additionally, the system utilizes the Twilio API to promptly notify the user's emergency contacts in case of a fall detection.

## Overview

The primary objective of Hermes Haven is to create a robust system for fall detection and immediate response for the urgent care of the elderly population. By analyzing kinematic data captured from various activities such as walking, sitting, standing, and falling, the system identifies patterns and features specific to falls to accurately detect and classify them.

## Features

- **Fall Detection Model:** Utilizes a linear SVM model trained on labeled kinematic data to predict falls based on learned patterns.
- **Threshold-Based Classifier:** Complements the SVM model with a threshold-based approach for improved accuracy in identifying sustained falls.
- **Twilio Integration:** Upon detecting a sustained fall, the system automatically triggers the Twilio API to place immediate calls to the user's designated emergency contacts.

## Dataset and Model Training

- **Dataset:** The system was trained using a diverse dataset comprising kinematic data collected from various activities, including falls from different angles. Falls were manually labeled within the dataset.
- **Training-Testing Split:** The dataset was divided into an 80% training set and a 20% testing set for model evaluation and validation.

## Usage

To use Hermes Haven, follow these steps:

1. **Data Collection:** Gather kinematic data using OpenCap sensors.
2. **Model Training:** Train the linear SVM model and threshold-based classifier using the collected dataset.
3. **Integration:** Integrate the trained models into the system.
4. **Real-time Monitoring:** Continuously monitor the incoming kinematic data for fall detection.
5. **Twilio Configuration:** Ensure Twilio API integration is properly set up to initiate calls to emergency contacts upon detecting a sustained fall.

   To see pre-existing runs, refer to the Notebook.

## Dependencies

Ensure the following dependencies are installed:

- Python (version 3.10.9)
- Libraries: NumPy, Pandas, Scikit-learn, Twilio, etc.

## License

This project is licensed under MIT License.
