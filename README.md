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

# Stock Price Trend Prediction with LSTM

## Objective
Predict future stock prices using past trends and technical indicators (MA50, MA200, RSI) with an LSTM model.

## Tools & Libraries
- Python 3.x  
- Pandas  
- NumPy  
- Matplotlib / Seaborn  
- yfinance API  
- TensorFlow / Keras  
- scikit-learn  
- TA-Lib / `ta` (for technical indicators)  
- Streamlit (optional, for dashboard)

## Project Steps

### 1. Fetch stock data
- Used `yfinance` to download historical stock data (Open, High, Low, Close, Volume).

### 2. Data preprocessing
- Calculated **technical indicators**:  
  - Moving Average (MA50, MA200)  
  - Relative Strength Index (RSI)  
- Scaled data using `MinMaxScaler` (0–1 range).  
- Prepared sequences of 60 timesteps for LSTM input.

### 3. Build LSTM model
- Multi-layer LSTM with dropout for regularization.  
- Input: sequences of 60 days × 4 features (Close, MA50, MA200, RSI).  
- Output: next day’s Close price.

### 4. Train & validate model
- Trained on historical data, validated with a small split.  
- Loss function: Mean Squared Error (MSE).  
- Epochs: 20, Batch size: 32 (adjustable).

### 5. Test & visualize predictions
- Prepared test sequences with indicators.  
- Predicted prices vs actual prices plotted using Matplotlib.  

### 6. Save model
- Saved full model: `lstm_stock_model.h5`  
- Can reload for inference without retraining.

### 7. Optional Streamlit dashboard
- Live prediction interface.  
- Input: stock ticker, days to predict.  
- Output: predicted next day stock price.

## Deliverables
- Jupyter/Colab notebook with full code  
- Trained model weights: `lstm_stock_model.h5`  
- Graphs: Actual vs Predicted stock prices  
- Streamlit dashboard (`app.py`) with live predictions  

## Usage

### Run Notebook
- Execute all cells sequentially in Google Colab.  

### Predict stock price in Streamlit
```bash
streamlit run app.py

Demonstrates NLTK usage, keyword matching, and category mapping

Expandable to dataset-based or UI-based versions

Perfect for a mini project submission in internship or academic settings
