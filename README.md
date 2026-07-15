# Custom Byte-Pair Encoding (BPE) Tokenizer from Scratch

## Project Overview

This project implements the Byte Pair Encoding (BPE) algorithm from scratch using Python and NumPy without using any external tokenization libraries. BPE is a subword tokenization technique widely used in Large Language Models (LLMs). The algorithm learns a vocabulary by repeatedly merging the most frequent adjacent symbol pairs.

## Objective

The objective of this project is to:

- Read and preprocess a text corpus.
- Split words into character-level tokens.
- Count word frequencies.
- Count adjacent symbol pair frequencies.
- Learn merge rules by repeatedly merging the most frequent pairs.
- Build a subword vocabulary.
- Implement custom `encode()` and `decode()` functions.
- Test the tokenizer on unseen words.

## Features

- Read text corpus
- Text preprocessing
- Character-level tokenization
- End-of-word (`</w>`) handling
- Word frequency calculation
- Adjacent pair frequency counting
- Pair merging
- Vocabulary updating
- Merge rule generation
- Final vocabulary construction
- Custom `encode()` function
- Custom `decode()` function
- Tokenizer testing

## Technologies Used

- Python 3
- NumPy
- Jupyter Notebook

## Project Structure

```
Custom_BPE_Tokenizer/
│
├── corpus.txt
├── BPE_Tokenizer.ipynb
└── README.md
```

## Algorithm Workflow

```
Start
   ↓
Read Corpus
   ↓
Preprocess Text
   ↓
Split Words into Characters + </w>
   ↓
Count Word Frequencies
   ↓
Find Adjacent Symbol Pairs
   ↓
Count Pair Frequencies
   ↓
Select Most Frequent Pair
   ↓
Merge Pair
   ↓
Update Vocabulary
   ↓
Repeat Until Required Number of Merges
   ↓
Store Merge Rules
   ↓
Build Final Vocabulary
   ↓
Encode New Words
   ↓
Decode Tokens
   ↓
End
```

## Learning Outcome

This project demonstrates how Byte Pair Encoding (BPE) learns subword tokens by repeatedly merging the most frequent adjacent symbol pairs. It provides a basic understanding of the tokenization process used in modern Large Language Models.

## Author

**JASCINTH RHEMA .R**

B.Sc. Computer Science with Artificial Intelligence

---

This project was developed for educational purposes to understand the Byte Pair Encoding (BPE) algorithm from scratch.
