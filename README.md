# Large Language Models Lab

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Notebooks-Jupyter-F37626?logo=jupyter&logoColor=white)
![PyTorch](https://img.shields.io/badge/Deep%20Learning-PyTorch-EE4C2C?logo=pytorch&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-1F883D)

A practical, end-to-end study of language models, starting with statistical text modeling and progressing through embeddings, recurrent networks, attention, and Transformer components.

This repository is designed to be read as an engineering progression: each experiment isolates a core idea, implements it in a notebook, and preserves the executed outputs and visual artifacts for review.

## What This Demonstrates

- Text cleaning, tokenization, vocabulary construction, and corpus statistics
- N-gram language modeling and probability-based text generation
- Word2Vec and FastText embeddings with similarity and analogy queries
- Hugging Face tokenization workflows and tokenizer comparison
- PyTorch dataset preparation, batching, training loops, and evaluation
- LSTM language modeling and sequence-to-sequence encoder-decoder models
- Attention-based sequence modeling with masking and gradient clipping
- Transformer building blocks: scaled dot-product attention, multi-head attention, positional encoding, layer normalization, and residual connections
- Reproducible notebook execution with saved outputs, plots, and tabular results

## Experiment Map

| Experiment | Focus | Main artifact |
| --- | --- | --- |
| [01 - N-gram language model](exp1/ngram_language_model.ipynb) | Corpus analysis, token frequencies, n-gram probabilities, and language-model fundamentals | [Corpus](exp1/corpus.txt) |
| [02 - Word embeddings](exp2/word_embeddings_gensim.ipynb) | Gensim Word2Vec and FastText, semantic similarity, analogies, and OOV behavior | Executed notebook outputs |
| [03 - Tokenization comparison](exp3/tokenization_comparison.ipynb) | Word-level and subword tokenization using modern NLP tooling | [Tokenization results](exp3/exp3_tokenization_results.csv) |
| [04 - LSTM language model](exp4/lstm_language_model.ipynb) | Sequence creation, embeddings, recurrent modeling, and next-token prediction | Executed PyTorch model output |
| [05 - Seq2Seq baseline](exp5/seq2seq_baseline.ipynb) | Encoder-decoder sequence modeling and teacher forcing | Executed training output |
| [06 - Seq2Seq with attention](exp6/seq2seq_attention.ipynb) | Attention weights, masking, training stability, and model comparison | Executed training output |
| [07 - Transformer encoder](exp7/transformer_encoder_from_scratch.ipynb) | Transformer components implemented step by step | [Training loss plot](exp7/copy_task_training_loss.png) and [positional encoding heatmap](exp7/positional_encoding_heatmap.png) |

The [course workbook](workbook/24AD07HF_LLMs_Lab_Workbook_Odd_Sem_2026-27.pdf) provides the lab context and experiment requirements.

## Repository Layout

```text
exp1/       Statistical language modeling
exp2/       Word embeddings with Gensim
exp3/       Tokenization experiments and CSV results
exp4/       LSTM language modeling
exp5/       Sequence-to-sequence baseline
exp6/       Attention-based sequence-to-sequence modeling
exp7/       Transformer encoder components and visualizations
workbook/   Course workbook used as the experiment reference
```

## Run Locally

```bash
git clone https://github.com/Hareesh-Reddy-9126/large-language-models-lab.git
cd large-language-models-lab

python -m venv .venv
# Windows: .venv\Scripts\activate
# macOS/Linux: source .venv/bin/activate

python -m pip install --upgrade pip
python -m pip install -r requirements.txt
python -m pip install jupyter
jupyter notebook
```

Open the experiment notebooks in numerical order. Most notebooks run on CPU, although PyTorch will use CUDA when it is available. Experiment 2 downloads large pretrained embedding models on first use, so it needs an internet connection and additional disk space.

## Reproducibility Notes

- The notebooks are committed with their executed outputs so the results can be reviewed directly on GitHub.
- Generated plots and the experiment 3 CSV are versioned alongside the notebooks.
- Notebook checkpoints and local editor metadata are excluded from version control.
- Results can vary slightly with library versions, random seeds, and available hardware.

## Skills Snapshot

**Python · PyTorch · NLP · Gensim · Hugging Face Transformers · NLTK · NumPy · Pandas · Matplotlib · Jupyter · Deep Learning Fundamentals**

## Author

**Hareesh Reddy**

GitHub: [@Hareesh-Reddy-9126](https://github.com/Hareesh-Reddy-9126)