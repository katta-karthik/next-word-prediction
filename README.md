# Next Word Prediction Using LSTM

## Overview
This project implements a next word prediction model using Long Short-Term Memory (LSTM) networks. The model is trained on Shakespeare's "Hamlet" and predicts the next word in a sequence.

## Features
- Trained on Shakespeare's "Hamlet" text
- LSTM-based neural network architecture
- Interactive web interface using Streamlit
- Real-time word prediction

## Installation
1. Clone the repository:
   git clone https://github.com/katta-karthik/next-word-prediction.git
   cd next-word-prediction

2. Create a virtual environment:
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate

3. Install dependencies:
   pip install -r requirements.txt

## Project Structure
.
├── app.py                 # Streamlit web application for predictions
├── experiemnts.ipynb     # Jupyter notebook containing model training code
├── requirements.txt      # List of Python dependencies
├── hamlet.txt           # Training dataset (Shakespeare's Hamlet)
├── README.md           # Project documentation
├── .gitignore         # Git ignore file
└── models/           # Directory containing trained models
    ├── next_word_lstm.h5    # Trained LSTM model
    └── tokenizer.pickle     # Fitted tokenizer

## Usage
1. Run the Streamlit app:
   streamlit run app.py
2. Enter a sequence of words in the text input field
3. Click "Predict Next Word" to see the prediction

## Model Architecture
- Embedding layer (100 dimensions)
- LSTM layer (150 units) with return sequences
- Dropout layer (0.2)
- LSTM layer (100 units)
- Dense output layer with softmax activation

## Training Data
The model is trained on Shakespeare's "Hamlet", providing a rich vocabulary and complex language patterns for the model to learn from.

## Contributing
Feel free to open issues or submit pull requests if you have suggestions for improvements.

## License
MIT License