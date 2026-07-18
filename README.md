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

# Custom Byte Pair Encoding (BPE) and Autoregressive Causal Language Model

## Project Overview

This project demonstrates the implementation of a **Custom Byte Pair Encoding (BPE) Tokenizer** and the preprocessing pipeline required for an **Autoregressive Causal Language Model (ARLM)** using **Python** and **NumPy**.

The objective is to understand how modern language models preprocess text and prepare data before training.

---

## Features

- Read a text corpus
- Preprocess text
- Count word frequencies
- Build initial character vocabulary
- Find adjacent character pairs
- Calculate pair frequencies
- Perform Byte Pair Encoding (BPE)
- Store learned merge rules
- Convert learned tokens into Token IDs
- Prepare data for an Autoregressive Causal Language Model

---

## Project Workflow

```
Raw Text
    │
    ▼
Read Corpus
    │
    ▼
Text Preprocessing
    │
    ▼
Word Frequency Calculation
    │
    ▼
Character-Level Vocabulary
    │
    ▼
Find Adjacent Character Pairs
    │
    ▼
Calculate Pair Frequencies
    │
    ▼
Merge Most Frequent Pair
    │
    ▼
Repeat Until Required Vocabulary Size
    │
    ▼
Learned BPE Vocabulary
    │
    ▼
Token IDs
    │
    ▼
Input–Target Pair Creation
    │
    ▼
Autoregressive Language Model
```

---

## Technologies Used

- Python 3
- NumPy
- Regular Expressions (re)
- Collections (Counter, defaultdict)
- Jupyter Notebook

---

## Project Structure

```
Custom_BPE_Autoregressive_Language_Model/

│── Custom_BPE_Autoregressive_Language_Model.ipynb
│── corpus.txt
│── README.md
```

---

## Implementation Steps

### Part 1 – Byte Pair Encoding (BPE)

- Choose a text corpus
- Read the corpus
- Preprocess the text
- Split words into characters
- Count word frequencies
- Build the initial vocabulary
- Find adjacent character pairs
- Count pair frequencies
- Select the most frequent pair
- Merge the selected pair
- Repeat the merge process
- Store merge rules

---

### Part 2 – Autoregressive Causal Language Model

- Convert BPE tokens into Token IDs
- Create Input–Target pairs
- Generate token embeddings
- Add positional encoding
- Apply causal masking
- Compute self-attention
- Pass through a linear layer
- Apply softmax
- Calculate cross-entropy loss
- Update model parameters
- Generate text iteratively

---

## Learning Outcomes

After completing this project, you will understand:

- How Byte Pair Encoding works
- Why subword tokenization is important
- How token IDs are generated
- Data preparation for language models
- The preprocessing pipeline of GPT-like models
- Fundamentals of autoregressive text generation

---

## Future Improvements

- Complete transformer implementation using NumPy
- Multi-head self-attention
- Feed Forward Network (FFN)
- Layer Normalization
- Model training
- Text generation using beam search or sampling

---

**JASCINTH RHEMA .R**

B.Sc. Computer Science with Artificial Intelligence

---

This project was developed for educational purposes to understand the Byte Pair Encoding (BPE) algorithm from scratch.
