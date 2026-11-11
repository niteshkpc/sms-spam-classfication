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
   python -m pip install streamlit nltk scikit-learn
   ```

2. Download the NLTK resources used for tokenization and stop words:

   ```bash
   python -c "import nltk; nltk.download('punkt'); nltk.download('punkt_tab'); nltk.download('stopwords')"
   ```

3. Start the app from the project directory:

   ```bash
   streamlit run app.py
   ```

4. Open the local URL printed by Streamlit, enter a message, and select **Predict**.

## Project files

- `app.py` — Streamlit interface and text preprocessing
- `model.pkl` — trained classification model
- `vectorizer.pkl` — fitted TF-IDF vectorizer used by the model
