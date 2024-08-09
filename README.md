# Youth Awards Programme - Natural Language Processing

NLP teaching material for the KCL Department of Biostatistics & Health Informatics Youth Awards Programme


## Exercise 1 - Shakespeare's plays as vectors
(Oriignal idea from [Jurafsky and Martin, Speech and Language Processing, Draft 3rd Edition](https://web.stanford.edu/~jurafsky/slp3/))

We will start by looking at how we might represent documents. We are going to do a simple analysis of Shakespeare's plays, which are available in digital form from a USA library, the [Folger Shakespeare Library](https://www.folger.edu/explore/shakespeares-works/download/). We will look at the plain text of four plays:

- [As You Like It](https://flgr.sh/txtfssAYLtxt)
- [Twelfth Night](https://flgr.sh/txtfssTN_txt)
- [Julius Caesar](https://flgr.sh/txtfssJC_txt)
- [Henry V](https://flgr.sh/txtfssH5_txt)


## Exercise 2 - Word context vectors

We will build word context vectors using the [iWeb corpus](https://www.english-corpora.org/iweb/), : a corpus of 14 billion words in 22 million systematically selected English language web pages. This can be searched and analysed using the tools at [English-Corpora.org](https://www.english-corpora.org/). We have used these tools to look at a few words, and to find what other words appear in their context (on the same web page). We have saved these in a spreadsheet, which has one sheet for each of our words:

- [Word context data](./contexts.xlsx) (click the "View raw" button to download, tnen open on your computer)

We have written a Python notebook to examine these words:

[Python notebook exercise](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main//plot_contexts.ipynb)

## Exercise 3 - Playing with word embeddings

[Word embedding exercise](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main/embeddings.ipynb)


## Exercise 4 - Building a perceptron

[Experiments with a single neuron](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main//perceptrons.ipynb)

## Exercise 5 - Multilayer Neural Networks

[Neural network playground](https://playground.tensorflow.org/)

## Exercise 6 - Generative AI

- [Connecting to Hugging Face](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main//hugging_face.ipynb)
- [Experiments with Llama](https://githubtocolab.com/KCL-Health-NLP/nlp_youth_awards/blob/main//llama.ipynb)
