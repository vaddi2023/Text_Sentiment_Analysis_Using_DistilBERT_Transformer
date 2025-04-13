Project:
Title: Text Sentiment Analysis Using Distilbert Transformer
This project implements a binary text sentiment classification system using the DistilBERT transformer model. The task involves identifying positive or negative sentiment in IMDB movie reviews.

Project Execution:
python -m venv sentiment_env
sentiment_env\Scripts\activate
pip install -r requirements.txt
pip install notebook
jupyter notebook

📌 Key Components
Dataset: A sampled subset of the IMDB Movie Reviews dataset, containing 50,000 reviews labeled as positive or negative.
Model: Fine-tuned DistilBERT, a lightweight version of BERT, used for efficient natural language understanding tasks.
Preprocessing: Includes lowercasing, punctuation removal, and handling of gibberish inputs.
Tokenization: Text data is preprocessed and tokenized using DistilBertTokenizerFast.
Model Training:
Framework: PyTorch
Loss Function: BCEWithLogitsLoss for binary classification
Optimizer: AdamW
Evaluation: Accuracy, Loss Curves, Confusion Matrix, and Classification Report
Thresholding: Custom threshold(0.50) applied on sigmoid output to convert to binary sentiment class.
Visualization: Includes training/validation loss & accuracy curves and sentiment label distribution.

⚙️ Techniques Used to improve performance:
Transfer Learning: Leveraging pretrained DistilBERT weights.
Early Stopping: Prevents overfitting by monitoring validation performance.
Hyperparameter Tuning: Batch size, learning rate, dropout rate, and epochs tuned for optimal performance.
