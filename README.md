🧠 Next Word Prediction with LSTM and Streamlit
This project demonstrates a Next Word Prediction application built using a Long Short-Term Memory (LSTM) neural network trained on Shakespeare’s Hamlet. The project uses Streamlit for the user interface, and a pre-trained LSTM model to predict the next word in a given text input.

<br>
📌 Features
🚀 LSTM-based next-word prediction

📚 Trained on The Tragedy of Hamlet by William Shakespeare

🧪 Clean and minimal Streamlit interface

✅ Early stopping used during training to avoid overfitting

🔠 Tokenizer saved and reused for inference

🗣️ Predicts the next most likely word for a given sequence

<br>
📁 Project Structure

├── app.py                # Streamlit web app <br>
├── tokenizer.pickle      # Tokenizer used during training<br>
├── next_word_lstm.h5     # Trained LSTM model<br>
├── hamlet.txt            # Training corpus (Hamlet by Shakespeare)<br>
├── experiemnts.ipynb     # Jupyter notebook for training/testing <br>
<br>
🧪 Demo
To be or not to → predicts: be

Just enter the first few words of a sentence and get the predicted next word!

<br>
▶️ Run Locally
Prerequisites
Python 3.7+

pip

Install dependencies
bash
Copy
Edit
pip install -r requirements.txt
Ensure you have these files in the same directory:

next_word_lstm.h5

tokenizer.pickle

app.py

Start the app
bash
Copy
Edit
streamlit run app.py
<br>
🧠 How it Works
Tokenizer: Text from hamlet.txt is tokenized and sequences are generated for training.

Model: An LSTM model is trained to predict the next word in a sequence.

Prediction:

Input text is tokenized and padded.

The model outputs probabilities for the next word.

The most likely word is decoded from the token index.

<br>
📚 Training Details
Dataset: hamlet.txt (Shakespeare)

Model: LSTM with embedding

Preprocessing: Keras Tokenizer, padding sequences

Training techniques:

EarlyStopping callback

Sequence length derived from tokenizer input

The training process is documented in experiemnts.ipynb.


<br>
📜 License
This project uses publicly available text and is free for educational and research purposes.
