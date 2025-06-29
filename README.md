# AI-CHATBOT

Transformer Chatbot
This is a Transformer-based chatbot built using PyTorch. The model is trained on a custom dataset of user queries and corresponding responses. It uses positional encoding, token embedding, and a full encoder-decoder Transformer architecture.

Features
--Encoder-Decoder Transformer architecture

--Custom tokenizer and vocabulary

--Training loop with accuracy tracking

--Positional encoding implemented from scratch

--Padded batching with PyTorch DataLoader

--Clean preprocessing pipeline

Dataset
-- The chatbot is trained on a CSV file named merged_cleaned-data.csv with the following columns:

-- query: User input or question

-- response: Bot's expected response

Training Performance
-- After 100 epochs, the model achieves:

-- Training Accuracy: ~96%

-- Training Loss: ~0.19

Requirements
-- Python 3.7+

-- PyTorch

-- scikit-learn

-- pandas

-- numpy

-- Install with:
pip install torch pandas numpy scikit-learn

 Model Architecture
Embedding Layer for source and target tokens

PositionalEncoding module

nn.Transformer with:

-- 4 Encoder & Decoder Layers

-- 8 Attention Heads

-- Feedforward Layer: 512 units
Output Linear layer for vocab prediction


Tokenization and Encoding
Tokens are lowercased, punctuation is removed

Tokens are converted to IDs using a vocabulary

Special tokens:

-- <pad>

-- <sos>

-- <eos>

-- <unk>

References
Vaswani et al., "Attention Is All You Need"

PyTorch nn.Transformer documentation
👤 Author
Bibhav Kumar and Riya Chettri
🌐 GitHub
