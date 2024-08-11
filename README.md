# Natural Language Processing

**Biostatistics and Health Infromatics Youth Awards Programme**

**King's College London Institute of Psychiatry, Psychology and Neuroscience**

---


- This repository contains all the material you will need for the NLP day on the Biostatistics and Health Informatics Youth Awards Programme
- The day will consist of six practicals introducing some topics in NLP and neural networks
- Each practical will be introduced by short presentations of around 5 minutes each

### Python

- Practicals will be in the Python programming language
- Don't worry if you don't know any Python, you do not need to write any code
- We will explain how to run the code, and talk you through each step
- We will run our Python code using Google Colaboratory (Colab), a cloud-based virtual compute service
- You will need a Gmail / Google account to use Colab

## Contents

1. [Introduction](#introduction)
2. [Generative AI](#generative-ai)

## Introduction

- Why NLP?
- 

## 2 - Shakespeare's plays as vectors
*Original idea from Jurafsky and Martin, [Speech and Language Processing](https://web.stanford.edu/~jurafsky/slp3/), Draft 3rd Edition.*

We will start by looking at how we might represent documents. We are going to do a simple analysis of Shakespeare's plays, which are available in digital form from a USA library, the [Folger Shakespeare Library](https://www.folger.edu/explore/shakespeares-works/download/). We will look at the plain text of four plays:

- [As You Like It](https://flgr.sh/txtfssAYLtxt)
- [Twelfth Night](https://flgr.sh/txtfssTN_txt)
- [Julius Caesar](https://flgr.sh/txtfssJC_txt)
- [Henry V](https://flgr.sh/txtfssH5_txt)

**Practical**

- Each person will be allocated a play from the above list, and a word
- Count the number of times your word occurs in your play
- A simple way to do this is to use CTRL-F in your browser - this finds words in a page
- The dialog box in which you type the search word will tell you how many times it occurs
- Take care with *wit* - it is also found in common words like *with* - how will you overcome this?
- Enter your results in [this spreadsheet](https://docs.google.com/spreadsheets/d/1W-NI1-CAufuXTCHISsbwvnqY5krQVnsAxqX2IKpNcVg/edit?usp=sharing)

## 2 - Vector semantics

We will build word context vectors using the [iWeb corpus](https://www.english-corpora.org/iweb/): a corpus of 14 billion words in 22 million systematically selected English language web pages. This can be searched and analysed using the tools at [English-Corpora.org](https://www.english-corpora.org/). We have used these tools to look at a few words, and to find what other words appear in their context (on the same web page). We have saved these in a spreadsheet, which has one sheet for each of our words:

- [Word context data](./contexts.xlsx) (click the "View raw" button to download, tnen open on your computer)

We have written a Python notebook to examine these words:

[Python notebook exercise](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main//plot_contexts.ipynb)

## 3 - Playing with word embeddings

[Word embedding exercise](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main/embeddings.ipynb)


## 4 - Building and training a single neuron (a perceptron)

[Experiments with a single neuron](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main//perceptrons.ipynb)

## 5 - Multilayer Neural Networks

[Neural network playground](https://playground.tensorflow.org/)

## Generative AI

- [Connecting to Hugging Face](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main//hugging_face.ipynb)
- [Experiments with Llama](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main//llama.ipynb)
