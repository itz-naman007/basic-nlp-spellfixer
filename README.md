# simple-spell-corrector

A minimal, sentence-level spelling correction tool built from scratch using basic NLP techniques. This project uses the [English Word Frequency dataset](https://www.kaggle.com/datasets/rtatman/english-word-frequency) to detect and correct common spelling mistakes in user input. It does not rely on any pretrained language models or external APIs.

---

## Features

- Custom spell checker built using Python
- Uses edit-distance operations (insertion, deletion, replacement, transposition)
- Ranks correction candidates based on word frequency
- Handles sentence-level input
- No deep learning, pretrained models, or third-party spell libraries

---

## How It Works

1. Loads the English Word Frequency list from Kaggle
2. Builds a vocabulary and calculates probabilities based on frequency
3. For each word in the input sentence:
   - If the word exists in the vocabulary, it's returned unchanged
   - Otherwise, all possible single-edit candidates are generated
   - The most probable valid word is selected as the correction

---
