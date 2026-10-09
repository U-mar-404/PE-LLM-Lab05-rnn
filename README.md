# Lab 05: Recurrent Neural Networks for Sequence Modeling

Course: Prompt Engineering and LLM Applications (BSAI, 7th Semester)

This lab uses SimpleRNN models for three sequence tasks: translation, sentiment analysis, and text generation.

## Tasks

| Task | Description | Dataset |
|------|-------------|---------|
| 1. Language Translation | Encoder-decoder SimpleRNN that translates short English sentences (3-6 words) into French | Tatoeba/Anki fra-eng (first 10,000 pairs) |
| 2. Sentiment Analysis | Multi-class (negative / neutral / positive) SimpleRNN classifier with softmax output | Twitter US Airline Sentiment |
| 3. Text Generation | Character-level SimpleRNN that generates text one character at a time with temperature sampling | Shakespeare text (about 1.1 MB) |

## Experiments

- **Task 1:** hidden units (64 / 128 / 256), embedding dimension (32 / 64 / 128), short vs longer sentences
- **Task 2:** max_length (20 / 40 / 80), units (32 / 64 / 128), dropout (0.2 / 0.5), with vs without class_weight
- **Task 3:** sequence length (25 / 50 / 100), units (64 / 128 / 256), temperature (0.2 / 0.7 / 1.2)

## Files

- `Prompt_Eng_Lab_5.ipynb`: notebook with code and outputs for all tasks
- `README.md`: this file

## How to Run

1. Open the notebook in Google Colab using the badge or link in the notebook.
2. Run the cells from top to bottom. Datasets are downloaded automatically.
3. An internet connection is required for the dataset downloads.

## Requirements

- Python 3
- TensorFlow / Keras
- NumPy, Pandas, Matplotlib, scikit-learn
