# NLP Labs Repository

Welcome to the **NLP_LABS** repository! This collection encompasses all the lab assignments I've completed during on of my Natural Language Processing introduction coursework. Each lab explores different facets of NLP, from foundational algorithms to advanced neural network architectures.

## Table of Contents

- [Lab 02: Naive Bayes Algorithm and Stemming](#lab-02-naive-bayes-algorithm-and-stemming)
- [Lab 03: Feature Engineering and Logistic Regression](#lab-03-feature-engineering-and-logistic-regression)
- [Lab 04: Custom GloVe Implementation and FastText](#lab-04-custom-glove-implementation-and-fasttext)
- [Lab 05: Implementing an RNN with PyTorch](#lab-05-implementing-an-rnn-with-pytorch)
- [Lab 06: Transformers and Decoding Methods](#lab-06-transformers-and-decoding-methods)
- [Lab 07: Fine-Tuning Pre-trained Models on IMDB Dataset](#lab-07-fine-tuning-pre-trained-models-on-imdb-dataset)
- [Lab 08: Dataset Analysis and Model Evaluation](#lab-08-dataset-analysis-and-model-evaluation)

---

## Lab 02: Naive Bayes Algorithm and Stemming

In this lab, we delve into:

- **Naive Bayes Classification**: Implemented the Naive Bayes algorithm for text classification tasks.
- **Stemming Techniques**: Explored various stemming methods to preprocess and normalize text data for improved model performance.

[Lab 02 Details](./02/)

---

## Lab 03: Feature Engineering and Logistic Regression

This lab focuses on:

- **Feature Extraction**: Identified and extracted significant features from textual data to enhance model learning.
- **Logistic Regression Classification**: Applied logistic regression for classification, analyzing its efficacy compared to other models.

[Lab 03 Details](./03/)

---

## Lab 04: Custom GloVe Implementation and FastText

Key components of this lab include:

- **Custom GloVe Implementation**: Built a custom implementation of the GloVe algorithm to generate word embeddings from scratch.
- **FastText Exploration**: Experimented with FastText for efficient text classification and word representation learning.

[Lab 04 Details](./04/)

---

## Lab 05: Implementing an RNN with PyTorch

In this lab, we:

- **Built an RNN from Scratch**: Created a Recurrent Neural Network using PyTorch, following these steps:
  - **Embedding Layer**: Transformed one-hot encoded vectors into dense embeddings.
  - **Hidden Layer Computation**:
    - First Matrix (**W**): Connected embeddings to the hidden layer (`embedding_size` → `hidden_size`).
    - Second Matrix (**U**): Linked the previous hidden state to the current one (`hidden_size` → `hidden_size`).
    - Activation Function: Applied the tanh function to combine inputs and previous states:
      \[
      h_t = \tanh(Wx_t + Uh_{t-1})
      \]
  - **Output Layer**:
    - Matrix (**V**): Mapped hidden states to the output (`hidden_size` → `output_size`).
  - **Initialization**: Initialized the hidden state using an `init_hidden` function.
- **Accuracy Calculation**: Evaluated the RNN's performance on test data.

[Lab 05 Details](./05/)

---

## Lab 06: Transformers and Decoding Methods

This lab is divided into several parts:

### Part 1: PyTorch Transformers Tutorial

- **Understanding Transformers**: Followed a tutorial from the PyTorch documentation to grasp the fundamentals of transformer architectures.

### Part 2: Theoretical Questions

- **Deep Dive into Concepts**: Answered theoretical questions regarding encoding mechanisms, parameter usage, and masking functions within transformers.

### Part 3: Implementation of Decoding Functions

- **Top-K Decoding**: Implemented the top-k sampling method to select the k most probable next words during text generation.
- **Top-P (Nucleus) Decoding**: Developed the top-p sampling method to choose words whose cumulative probability meets a specified threshold p.

### Part 4: BLEU Score Evaluation

- **Model Evaluation**: Used the BLEU (Bilingual Evaluation Understudy) metric to assess the quality of generated text.
- **SacreBLEU Integration**: Leveraged the `corpus_score()` function from SacreBLEU for consistent and reliable scoring across experiments.

[Lab 06 Details](./06/)

---

## Lab 07: Fine-Tuning Pre-trained Models on IMDB Dataset

Activities in this lab include:

- **Fine-Tuning**: Adapted a pre-trained Hugging Face model to the IMDB movie reviews dataset, optimizing for both loss and accuracy.
- **Evaluation and Analysis**:
  - Assessed the fine-tuned model's performance.
  - Analyzed misclassified instances to identify patterns and potential improvements.
  - Answered theoretical questions related to NLP models and fine-tuning processes.

[Lab 07 Details](./07/)

---

## Lab 08: Dataset Analysis and Model Evaluation

This lab covers:

### Part 1: Selecting a Labeled Dataset

- **Legal Considerations**: Reviewed the legal implications of using publicly available datasets, focusing on proper licensing and ethical use.
- **Dataset Selection**: Chose an appropriate labeled dataset from the Hugging Face Hub for our analysis.

### Part 2: Evaluating the Dataset

- **Data Exploration**: Analyzed the distribution of classes and identified prevalent topics within the dataset.
- **Quality Assessment**: Checked for data biases and inconsistencies to ensure robustness in model training.

### Part 3: Evaluating a Pre-trained Model

- **Model Selection**: Opted to use the pre-trained RoBERTa model to save on computational resources.
- **Performance Metrics**:
  - Calculated precision, recall, and F1-score to evaluate model effectiveness.
  - Conducted tests on our own production data to gauge real-world applicability.
- **Comparison with Baseline Models**: Benchmarked RoBERTa against simpler models, like Naive Bayes, to contextualize its performance gains.

### Part 4: Annotation of Production Data

- **Golden Dataset Creation**: Compiled a high-quality annotated dataset by:
  - Internally annotating samples following a strict guideline.
  - Ensuring annotations are consistent and accurate.
- **Model Testing**: Used the golden dataset to rigorously test the pre-trained model's suitability for production use.

[Lab 08 Details](./08/)

---

## Getting Started

Each lab folder contains:

- **Detailed Instructions**: Step-by-step guides to understand and replicate the experiments.
- **Source Code**: All scripts and notebooks used for implementations.
- **Results**: Outputs, metrics, and analyses from the experiments.

---
