# Text Summarizer

An abstractive text summarization model built using an LSTM-based Encoder-Decoder architecture with attention mechanism.

## Dataset

The project uses the Inshorts News Dataset containing 5,000 news articles along with their corresponding headlines.

## Project Structure

1. Data Loading and Cleaning - Removed unnecessary columns and null values
2. Text Preprocessing - Cleaning, tokenization, and sequence padding for both encoder and decoder
3. Model Architecture - Encoder-Decoder LSTM with Additive Attention (Bahdanau Attention)
4. Model Training - Trained with early stopping to prevent overfitting
5. Inference - Separate encoder and decoder inference models for sequence generation
6. Evaluation - Tested on unseen news articles to generate predicted headlines

## Model Architecture

- Encoder: Embedding layer followed by LSTM
- Decoder: Embedding layer followed by LSTM with attention over encoder outputs
- Attention: Bahdanau (Additive) Attention mechanism
- Output: TimeDistributed Dense layer with softmax activation

## Libraries

- Python
- TensorFlow / Keras
- Pandas
- NumPy
- NLTK
- BeautifulSoup
