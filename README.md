# Natural Language Processing

**Biostatistics and Health Infromatics Youth Awards Programme**

**King's College London Institute of Psychiatry, Psychology and Neuroscience**

---

## Contents

1. [Introduction](#introduction)
1. [Representing language: documents](#representing-language-documents)
1. [Representing words: vector semantics](#representing-words-vector-semantics)
1. [Playing with word embedding](#playing-with-word-embeddings)
1. [Neural networks](#neural-networks)
1. [Generative AI](#generative-ai)

## Introduction
[[back to top]](#start-of-content)

- This repository contains all the material you will need for the NLP day on the Biostatistics and Health Informatics Youth Awards Programme
- The day will consist of six practicals to explore topics in NLP and neural networks
- Each practical will be introduced by short presentations of around 5 minutes each

**Python**

- Practicals will be in the Python programming language
- Don't worry if you don't know any Python, you do not need to write any code
- We will explain how to run the code, and talk you through each step
- We will run our Python code using Google Colaboratory (Colab), a cloud-based virtual compute service
- You will need a Gmail / Google account to use Colab
- If you do not have a Gmail account, [please create one now](https://support.google.com/mail/answer/56256?hl=en-GB) 

**Presentation**

- [Introductory presentation](./presentations/introduction.pdf) 

## Representing language: documents
[[back to top]](#start-of-content)

**Shakespeare's plays as vectors**
*Original idea from Jurafsky and Martin, [Speech and Language Processing](https://web.stanford.edu/~jurafsky/slp3/), Draft 3rd Edition.*

If we want to manipulate and analyse language computationally, we first need to find a way to represent language. We will start by looking at how we might represent documents. We are going to do a simple analysis of Shakespeare's plays, which are available in digital form from a USA library, the [Folger Shakespeare Library](https://www.folger.edu/explore/shakespeares-works/download/). We will look at the plain text of four plays:

- [As You Like It](https://flgr.sh/txtfssAYLtxt)
- [Twelfth Night](https://flgr.sh/txtfssTN_txt)
- [Julius Caesar](https://flgr.sh/txtfssJC_txt)
- [Henry V](https://flgr.sh/txtfssH5_txt)

**Practical**

- Each person will be allocated a play from the above list, and a word
- Count the number of times your word occurs in your play
- A simple way to do this is to use CTRL-F in your browser - this finds words in a page
- The dialog box in which you type the search word will tell you how many times that word occurs in the page
- Record your results in [this spreadsheet](https://docs.google.com/spreadsheets/d/1W-NI1-CAufuXTCHISsbwvnqY5krQVnsAxqX2IKpNcVg/edit?usp=sharing)

**Questions**

- *Wit* is also found in common words like *with* - how will you overcome this?
- Can we tell the difference between Shakespeare's comedies (e.g. As You Like It, Twelfth Night) and other plays?
- How might you represent a document?
- How might you visualise this?
- Can you think of any uses for this document representation?
- Can you think of a way to represent words?

## Representing words: vector semantics
[[back to top]](#start-of-content)

We've seen how to represent documents as vectors, but what about words themselves? 

**Presentation and demonstration**  

- [Presentation: distributional semantics](./presentations/distributional-semantics.pdf) 

We will demonstrate the idea of using a word's context to create a representation of that word by using a linguistic search engine, [WebCorp](https://www.webcorp.org.uk/). WebCorp allows us to find and list all contexts on the web in which a word appears, and to count the number of times other words appear next to it. We call these the the word's collocates).

- [Demonstration: WebCorp](https://www.webcorp.org.uk/)

**Practical**

This practical builds word vectors using data from the [iWeb corpus](https://www.english-corpora.org/iweb/): a corpus of 14 billion words in 22 million systematically selected English language web pages. This can be searched and analysed using the tools at [English-Corpora.org](https://www.english-corpora.org/). We have used these tools to look at a few words, and to find what other words appear in their context. In this case, we define context as being on the same web page. We have saved the context counts in a spreadsheet, which has one sheet for each of our words:

- [Word context data](./practicals/contexts.xlsx) (click the "View raw" button to download, tnen open on your computer)

You can use this spreadsheet with the Python notebook below to build and explore some word vectors:

- [Vector semantics - Python notebook](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main/practicals/plot_contexts.ipynb)

## Playing with word embeddings
[[back to top]](#start-of-content)

The simple word and document vectors we built above can be used in NLP and information retrieval applications, but they have a few shortcomings, and better distributional semantics solutions exist: **word embeddings**. Whereas the vectors we have looked at so far are high dimensional with integer values, word embeddings are much lower dimensional (maybe a few hundred dimensions), with real number values. The most popular of these is Google's [Word2Vec](https://www.tensorflow.org/text/tutorials/word2vec) and Stanford University's [GloVe](https://nlp.stanford.edu/projects/glove/). We will use both of these in the practical below.

**Presentation**
- [Word embeddings](./presentations/word-embeddings.pdf) 

**Practical**

- [Word embeddings - Python notebook](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main/practicals/embeddings.ipynb)


## Neural networks
[[back to top]](#start-of-content)

**Presentation**
- [Neural networks](./presentations/neural-networks.pdf) 


**Practicals**
- [Experiments with a single neuron](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main/practicals/perceptrons.ipynb)
- [Neural network playground](https://playground.tensorflow.org/)

## Generative AI
[[back to top]](#start-of-content)

**Presentation**
- [Transformers and generative AI](./presentations/transformers.pdf) 

**Practicals**
- [Connecting to Hugging Face](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main/practicals/hugging_face.ipynb)
- [Experiments with Llama](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main/practicals/llama.ipynb)
