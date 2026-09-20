# IMDB-Movie-Review-Sentiment-Analysis-Simple-RNN-
A Streamlit web app that classifies movie reviews as Positive or Negative using a Simple RNN trained on the IMDB dataset.

Project Structure
├── main.py               # Streamlit app
├── simple_rnn_imdb.h5    # Pre-trained model
├── requirements.txt      # Dependencies
└── README.md
Setup

Requires Python 3.10 (TensorFlow 2.15.0 supports Python 3.9 to 3.11).

bash
git clone this repo
cd the repo
conda create -n rnn python=3.10 -y
conda activate rnn
pip install -r requirements.txt
Run
bash
streamlit run main.py

Open http://localhost:8501, enter a movie review, and click Classify.

How It Works

The review is tokenized, converted to integers using the IMDB word index, padded to 500 tokens, and passed to the RNN. A score above 0.5 is labeled Positive, otherwise Negative.
