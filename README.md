# Byte Pair Encoding (BPE) Tokenizer

A Python implementation of the **Byte Pair Encoding (BPE)** algorithm from scratch. This project demonstrates how BPE learns subword vocabularies by repeatedly merging the most frequent adjacent character pairs. The implementation also supports encoding new words into subword tokens and decoding them back into their original form.

---

## Overview

Byte Pair Encoding (BPE) is a popular subword tokenization algorithm used in Natural Language Processing (NLP). Instead of treating every word as a unique token, BPE learns common character sequences and creates subword units, making it effective for handling rare and unseen words.

This project implements the complete BPE workflow without using any external NLP libraries.

---

## Features

- Character-level vocabulary construction
- Word frequency calculation
- Adjacent symbol pair frequency counting
- Most frequent pair selection
- Iterative pair merging
- Merge rule generation
- Final subword vocabulary creation
- Word encoding into subword tokens
- Token decoding back into original words

---

## Project Structure

```
Byte-Pair-Encoding/
│
├── bpe_tokenizer.py
├── README.md
```

---

## Algorithm Workflow

1. Create a text corpus.
2. Build a character-level vocabulary.
3. Count adjacent symbol pair frequencies.
4. Select the most frequent symbol pair.
5. Merge the selected pair.
6. Update the vocabulary.
7. Repeat merging for a fixed number of iterations.
8. Store merge rules.
9. Build the final vocabulary.
10. Encode new words.
11. Decode tokens back to text.

---

## Technologies Used

- Python 3
- NumPy
- collections.Counter

---

## Sample Corpus

```
study
student
students
studying
teach
teacher
teaching
taught
learn
learner
learning
learned
```

---

## Sample Encoding

**Input**

```
learning
```

**Encoded Output**

```
['learn', 'i', 'n', 'g', '</w>']
```

---

## Sample Decoding

**Input**

```
['learn', 'i', 'n', 'g', '</w>']
```

**Output**

```
learning
```

---

## Applications

- Natural Language Processing (NLP)
- Large Language Models (LLMs)
- Machine Translation
- Text Tokenization
- Chatbots
- Search Engines
- Speech Recognition

---

## Future Enhancements

- Read corpus from a text file
- Export learned vocabulary
- Save merge rules
- Support larger datasets
- Improve encoding efficiency
- Visualize merge operations

---

## Author

**Devi Sree**

B.Sc. Computer Science with Artificial Intelligence

