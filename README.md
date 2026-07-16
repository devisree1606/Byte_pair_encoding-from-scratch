# Byte Pair Encoding (BPE) Tokenizer

A Python implementation of the **Byte Pair Encoding (BPE)** algorithm for learning subword vocabularies and performing tokenization. This project demonstrates how BPE iteratively merges the most frequent symbol pairs to create a compact vocabulary, a technique widely used in modern Natural Language Processing (NLP) models.

---

## Overview

Byte Pair Encoding (BPE) is a data compression-inspired algorithm adapted for NLP to efficiently tokenize text into subword units. Instead of treating every word as a unique token, BPE learns frequently occurring character sequences, allowing models to handle unseen or rare words more effectively.

This implementation includes the complete BPE workflow:

- Character-level vocabulary construction
- Adjacent pair frequency calculation
- Iterative pair merging
- Merge rule generation
- Vocabulary creation
- Word encoding
- Token decoding

---

## Features

- Character-level vocabulary initialization
- Frequency-based pair selection
- Automatic merge rule learning
- Configurable number of merge operations
- Subword token generation
- Token decoding back to original text
- Simple and well-structured Python implementation

---

## Project Structure

```
.
├── bpe.py
└── README.md
```

---

## Algorithm Workflow

1. Build an initial character-level vocabulary.
2. Count the frequency of adjacent symbol pairs.
3. Select the most frequent pair.
4. Merge the selected pair across the vocabulary.
5. Repeat for the specified number of merge iterations.
6. Store learned merge rules.
7. Encode unseen words using the learned vocabulary.
8. Decode tokens back into readable text.

---

## Technologies Used

- Python 3
- NumPy
- collections.Counter

---

## Example

### Input

```
drive
driver
driving
code
coder
coding
learn
learner
learning
```

### Encoding

```
Original : learning
Encoded  : ['learn', 'i', 'n', 'g', '</w>']
```

### Decoding

```
Decoded : learning
```

---

## Applications

- Natural Language Processing
- Large Language Models (LLMs)
- Machine Translation
- Text Tokenization
- Vocabulary Learning
- Language Modeling

---

## Future Improvements

- Support for larger text corpora
- File-based corpus loading
- Vocabulary export/import
- Performance optimization
- Visualization of merge operations

---

## Author

**Devi Sree.T**

B.Sc. Computer Science with Artificial Intelligence

---

## License

This project is provided for educational and research purposes.
