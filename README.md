Abstract

Road accidents are a leading cause of fatalities worldwide. 
Quick detection and reporting are crucial for timely emergency response. 
This project presents a deep learning–based accident detection system that uses Convolutional Neural Networks (CNN) to analyze video footage and classify frames as 
either 'Accident' or 'No Accident'. Built with tools like OpenCV, TensorFlow, and Keras, 
the system processes frames extracted from videos, performs feature extraction using VGG16, and applies a trained model to detect incidents in real-time or post-event analysis.
With optional Twilio SMS integration, this solution can alert emergency contacts instantly, making it suitable for deployment in smart traffic surveillance systems.

Project Features

- Video-to-frame extraction using OpenCV  
- Accident classification using VGG16 CNN model  
- Image preprocessing with skimage and TensorFlow utilities  
- Real-time prediction output: “Accident” or “No Accident”  
- Ready for Twilio SMS integration for instant emergency alerts  
- Model training and accuracy validation using train-test split  
- Visual analytics via Matplotlib  


Requirements

- Python (Anaconda distribution recommended)  
- Required Libraries:  
  - OpenCV  
  - NumPy  
  - Pandas  
  - Matplotlib  
  - TensorFlow / Keras  
  - scikit-image (skimage)  
  - Geopy (optional)  
  - Twilio (optional for SMS alerts)  
- Dataset:  
  - `mapping.csv` (for training)  
  - `test.csv` (for prediction)  

How it Works

1. Extracts frames from an input video file using OpenCV.  
2. Preprocesses images: resize, scale, and format using skimage and Keras tools.  
3. Labels are one-hot encoded using to_categorical.  
4. Features are extracted using VGG16 without the top layer.  
5. Flattened features are used to train a fully connected neural network.  
6. Test frames are classified, and results are printed or sent via SMS (if integrated).  

Project Developed By
- Bhagyashree Jadhav  
- Shubham Shinde
