# Smart-Waste-Segregation-System

An AI-powered web application that automatically classifies waste materials into 12 categories and provides tailored recycling guidance to promote sustainable waste management practices.

## Features

- **Image Classification**: Upload images or use live camera to identify waste
- **AI-Powered**: Deep learning model based on MobileNetV2 architecture
- **Recycling Guidance**: Detailed recycling methods for each waste category
- **Location-Based**: Find recycling centers in your state
- **QR Integration**: Quick access to recycling centers via QR codes
- **Camera Support**: Real-time waste classification using device camera
- **Confidence Scores**: Transparent AI predictions with probability percentages
- **Web-Based**: Accessible from any device with a browser

## Waste Categories Classified

1. Battery
2. Biological/Organic Waste
3. Brown Glass
4. Cardboard
5. Clothes/Textiles
6. Green Glass
7. Metal
8. Paper
9. Plastic
10. Shoes
11. Trash (Non-recyclable)
12. White Glass

## Tech Stack

### Frontend
- **Streamlit** - Web application framework
- **OpenCV** - Image processing and computer vision
- **QRCode** - QR code generation for recycling centers

### Backend & AI/ML
- **TensorFlow** - Machine learning framework
- **Keras** - Deep learning API
- **MobileNetV2** - Pre-trained CNN model for transfer learning
- **NumPy** - Numerical computing and array processing

### Deployment
- **Streamlit Sharing** - Cloud deployment platform
- **GitHub** - Version control and code hosting

## Installation

### Prerequisites
- Python 3.8 or higher
- pip (Python package manager)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/Smart-Waste-Segregation-System.git
   cd Smart-Waste-Segregation-System

**Usage**

Choose Input Method: Select between image upload or camera capture

Provide Waste Image: Upload a clear image or use your camera to capture waste

Get Classification: AI model predicts the waste category with confidence score

View Recycling Guidance: Get detailed recycling instructions for the identified waste

Find Recycling Centers: Locate nearby recycling facilities using the interactive map

**Model Training**

The classification model was trained using transfer learning with MobileNetV2 as the base model:

Dataset: Garbage Classification Dataset from Kaggle (https://www.kaggle.com/datasets/mostafaabla/garbage-classification)

Classes: 12 waste categories

Input Size: 224×224 pixels

Preprocessing: Image normalization (0-1 scaling)

Augmentation: Rotation, flipping, zooming, and shifting

Training: Fine-tuning with custom classification layers

Validation: 80-20 split with early stopping
