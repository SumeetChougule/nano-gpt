# nanoGPT

nanoGPT is a minimal implementation of a decoder-only Transformer based on the paper ["Attention is All You Need"](https://arxiv.org/abs/1706.03762). This project is inspired by Andrej Karpathy's tutorial and is designed to pre-train on Shakespeare's text using a character-level tokenizer.

## Features

- Implementation of a decoder-only Transformer from scratch
- Character-level tokenization for training on Shakespeare's text
- Simple and clear code structure for educational purposes

## Getting Started

### Prerequisites

- Python 3.8 or higher
- PyTorch 1.8.0 or higher

### Installation

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/SumeetChougule/nano-gpt.git
cd nano-gpt
```

### Data Preparation

The model is trained on Shakespeare's text, which is available [here](https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt). Download the data using the following command:

```bash
wget https://raw.githubusercontent.com/karpathy/char-rnn/master/data/tinyshakespeare/input.txt -O data/input.txt
```

### Training

To train the model, run:

```bash
python nano_gpt.py
```

You can adjust the hyperparameters and training settings in the `nano_gpt.py` script.


## Code Overview

### Model

The Transformer model is implemented in `nano_gpt.py`. It consists of the following main components:

- `Embedding`: A simple embedding layer to convert input tokens into embeddings.
- `MultiHeadAttention`: Multi-head self-attention mechanism.
- `FeedForward`: Feed-forward network.
- `Block`: A single block of the Transformer consisting of multi-head attention and feed-forward layers.
- `Transformer`: The full decoder-only Transformer model.


## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.


## Acknowledgements

- [Andrej Karpathy](https://karpathy.ai/) for his insightful tutorial and inspiration for this project.
- The authors of the paper ["Attention is All You Need"](https://arxiv.org/abs/1706.03762) for their groundbreaking work on the Transformer model.
