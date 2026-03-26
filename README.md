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

# AI Virtual Career Counsellor
## Objective

Build an NLP-based chatbot to suggest career paths based on user interests

Handle multiple categories of interests (Tech, Arts, Commerce, Medicine, Law, Sports)

Demonstrate basic NLP techniques using NLTK

## Tools Used

Python

NLTK (Natural Language Toolkit)

PorterStemmer for keyword normalization

Command-line / IDLE interface

## Techniques Applied

Defined categories and keywords for different career domains

Used NLTK PorterStemmer to normalize user input and keywords

Implemented keyword matching to classify user interests

Created a looped input system to handle multiple queries

Provided career suggestions based on matched category

Error handling for unmatched interests

Designed to be expandable for future categories and keywords

## Evaluation

Tested with multiple user inputs:

I like coding and AI → suggested Tech careers

I enjoy painting and drawing → suggested Arts careers

Successfully mapped user interests to appropriate career suggestions

Works in any Python environment without external datasets


## Final Outcome

Functional AI career guidance bot

Demonstrates NLTK usage, keyword matching, and category mapping

Expandable to dataset-based or UI-based versions

Perfect for a mini project submission in internship or academic settings
