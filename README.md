# SMS Spam Classifier

A small Streamlit app that classifies a text message as **Spam** or **Not Spam**. It preprocesses the message with NLTK, converts it with the saved TF-IDF vectorizer, and predicts with the saved classifier.

## Requirements

- Python
- Streamlit
- NLTK
- scikit-learn

The trained model and vectorizer are included as `model.pkl` and `vectorizer.pkl`.

## Run locally

1. Install the required packages:

   ```bash
   python -m pip install -r requirements.txt
   ```

2. Start the app from the project directory:

   ```bash
   streamlit run app.py
   ```

3. Open the local URL printed by Streamlit, enter a message, and select **Predict**. The app downloads its required NLTK resources on first run if they are missing.

## Project files

- `app.py` — Streamlit interface and text preprocessing
- `model.pkl` — trained classification model
- `vectorizer.pkl` — fitted TF-IDF vectorizer used by the model
