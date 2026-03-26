# Face Mask Detection with Live Alert System

## Project Overview
This project detects whether people are wearing face masks in real-time using computer vision and deep learning. It uses a Convolutional Neural Network (CNN) to classify images of faces as either **Mask** or **No Mask**, and simulates live alerts for unmasked faces.

---

## Features
- Detects masked and unmasked faces in images
- High accuracy model trained on Kaggle dataset
- Simulated real-time detection using sample images
- Optional deployment with Flask for live webcam monitoring

---

## Folder Contents
- `face_mask_demo.ipynb` → Colab notebook containing all code: dataset preprocessing, model training, and demo  
- `mask_detector.h5` → Trained CNN model  
- `with_mask/` → Sample images of people wearing masks  
- `without_mask/` → Sample images of people without masks  
- `Face_Mask_Report.pdf` → 2-page report of the project  
- `requirements.txt` → Python packages required to run the project  

---

## How to Run
1. Open `face_mask_demo.ipynb` in **Google Colab**.  
2. Run all cells sequentially.  
3. Sample images will be labeled as **Mask** or **No Mask**.  
4. Optional: Use `mask_detector.h5` to skip retraining and directly test the model.  

---

## Tools & Libraries Used
- Python 3.x  
- TensorFlow / Keras  
- OpenCV  
- Haar Cascades for face detection  
- Matplotlib (for image display)  
- Google Colab

---

## Author
Rushita Bhosale  

---

## Notes
- Video demo is optional — screenshots from the Colab demo are sufficient for submission.  
- Ensure all sample images are included to make the demo reproducible.
