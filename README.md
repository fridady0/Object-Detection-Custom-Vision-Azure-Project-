# 🚗 Azure Custom Vision Object Detection Project

# Introduction

This project demonstrates how to build an Object Detection Model using Microsoft Azure’s Custom Vision service.
Unlike classification (which identifies what an image contains), object detection identifies where specific objects are located within an image.

The project uses a Car Object Detection Dataset to train, evaluate, and test a model capable of detecting cars in various images.
This tutorial provides a complete, step-by-step guide from dataset preparation to model evaluation and testing.

# 🎥 Project Demo

# 👉 Watch the Full Tutorial on YouTube: https://www.youtube.com/watch?v=HY2Y0BfD8aY


# Features

- Upload and label custom object detection datasets
- Train an object detection model using Azure Custom Vision
- Evaluate model performance with Precision, Recall, and Mean Average Precision (mAP)
- Test the model using local images or image URLs
- Deploy or export trained models for application integration
- Simple, visual workflow — no complex code required

# Setup & Installation

To set up the project, follow these steps:

- Sign in to the Azure Portal → https://portal.azure.com
- Create new Custom Vision resources:
- Resource Group: Create a new one (e.g., customvision-objectdetection01)
- Training Resource: Standard (or Free if available)
- Prediction Resource: Standard
- Deploy your resources.

-> Navigate to https://customvision.ai and sign in with your Azure account.

Create a New Project:

Name: Car Object Detection

Type: Object Detection

Domain: General [A1] (optimized for speed and performance)

# Dataset

The dataset consists of car images from multiple angles and scenes, used for object detection training.

Dataset Source: Provided by Kaizen for educational purposes.
Dataset Details:
Total Images Used : ~ 44

Images Used for Training: ~17–18
Tag Used: “Car”

⚠️ Note: A minimum of 15 tagged images is required to start model training.

#  Training Process

- Upload training images to your project.
- Create a tag named “Car”.
- Label the objects by drawing bounding boxes around cars in each image.
- Choose Quick Training (for smaller datasets) or Advanced Training (for more accuracy).
- Once training completes, Custom Vision displays model metrics:
- Precision → Measures accuracy of predictions
- Recall → Measures how many real objects were detected
- mAP (Mean Average Precision) → Overall detection performance

📈 Example Results:

Precision: 83%
Recall: 100%
Mean Average Precision: 100%
Even with a small dataset, the model performed exceptionally well.

# Testing & Evaluation

You can test the trained model in two ways:

- Local Image Upload:
  Upload a local image (e.g., containing one or multiple cars).

Example: Two cars → Model predicted both with 99.9% probability

- Image URL:
  Paste an online image URL directly into Custom Vision for live testing.

Example: Model detected cars in web images with 98–99% confidence

🔍 The model even differentiates between actual cars and background objects, showing lower confidence for false positives (e.g., humans or bikes).

# Deployment & Export

Once the model performs satisfactorily:
Publish the model to generate Prediction Endpoints
Integrate the model into applications using Azure Prediction API
Optionally, export the trained model to:
TensorFlow
ONNX
CoreML
Docker
or Edge devices
This makes it possible to use your model in mobile or real-time applications.

# Project Structure
```
[Azure Portal]
     │
     ▼
Create Custom Vision Resource
     │
     ▼
[CustomVision.ai Website]
     │
     ▼
Create Project → (Type: Object Detection / Domain: General A1)
     │
     ▼
Upload Dataset → Tag Object (Car)
     │
     ▼
Train Model → (Quick or Advanced Training)
     │
     ▼
Evaluate Model → Precision / Recall / mAP
     │
     ▼
Test Model → (Local Upload / Image URL)
     │
     ▼
Publish Model → Get Endpoint & Keys
     │
     ▼
(Optional) Export Model → TensorFlow / Docker / ONNX
```

# Model Performance Metrics
Metric	Description	Example Value
Precision	How accurate predictions are	83%
Recall	How many actual objects were found	100%
mAP	Average detection performance	100%

# Code of Conduct

This project follows the Contributor Covenant Code of Conduct.
By contributing or using this project, you agree to maintain a respectful and inclusive environment.

# License

This project is licensed under the MIT License.
You are free to use, modify, and distribute this project with proper attribution.

# 🙏 Acknowledgments

Special thanks to Kaizen for providing the Car Object Detection Dataset, which made this project possible.

⚠️ Note: This dataset and project are used strictly for educational and demonstration purposes to showcase the capabilities of Azure Custom Vision AI.

# 🌐 Useful Links

🔗 Azure Custom Vision Portal
🔗 Azure Portal
🔗 Microsoft Cognitive Services
🎥 YouTube Tutorial
