# word2vec-numpy

## Test task for JetBrains Internship Application
### Gregory Polyakov, 2026

This repository contains implementation of word2vec algorithm using pure numpy.
The implementation is based on the original papers ["Distributed Representations of Words and Phrases and their Compositionality", Mikolov et al., 2013](https://arxiv.org/abs/1310.4546), ["Efficient Estimation of Word Representations in Vector Space", Mikolov et al., 2013](https://arxiv.org/abs/1301.3781) and the original C implementation https://github.com/tmikolov/word2vec.

This implementation is based on CBOW architecture with negative sampling and includes the following features originally proposed by the authors:
- Learning rate decay
- Subsampling of frequent tokens
- Negative sampling according to token frequencies
- Random context window size

The dataset used for training is the [WikiText-103](https://huggingface.co/datasets/Salesforce/wikitext). It consists of over 100 million tokens extracted from Wikipedia articles.

### Installation

This project requires Python 3.11 or higher. The required dependencies can be installed via pip:

```bash
pip install -r requirements.txt
```

### Project Structure

- All the main code is located in the [`word2vec.ipynb`](word2vec.ipynb) Jupyter notebook.
- All the mathematical derivations of computing loss function and gradients are provided in the [`math_derivations.pdf`](math_derivations.pdf) (source TeX file: [`math_derivations.tex`](math_derivations.tex)).
- Trained model artifacts, including tokenized datase, trained embeddings, and loss logs.


