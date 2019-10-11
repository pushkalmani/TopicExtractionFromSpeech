# topicModelling
# Topic Modelling from speech 

### List of contents

- [Introduction](#introduction)
- [Working](#working)
- [Installation](#installation)
- [Running](#running)


## Introduction
---
[(Back to top)](#list-of-contents)

Topic Modelling is different from rule-based text mining approaches that use regular expressions or dictionary based keyword searching techniques. It is an unsupervised approach used for finding and observing the bunch of words (called “topics”) in large clusters of texts.

## Working
---
[(Back to top)](#list-of-contents)

The step-by-step procedure of the Project:

+ Conversion of Audio file to Text :-The first stage is to convert audio to text and we would be using two strategies . 
first converting audio file of wav format  to text using pyaudio and Google Speech Recognition and the second one is speaking through mic and converting that audio into text , in the second case the speaker while speaking can pause for 180 seconds and it will not affect the recording of audio .


+ Preparing text for topic modelling 
Tokenize words and cleanup text 
1. Tokenize each sentence into a list of words, removing punctuations and unnecessary characters altogether.
2. Creating BIgrams and trigrams model :- Bigrams are two words frequently occurring together in the document. Trigrams are 3 words frequently occurring.
3. Remove stopwords, make bigrams and lemmatize.

4. Create the Dictionary and Corpus needed for Topic Modeling.

+ Building Topic Model :- We have everything required to train the LDA model. In addition to the corpus and dictionary, you need to provide the number of topics as well.


+ Compute Model perplexity and Coherence Scores.
+ To analyse what is the optimal number of topics in the text document we have to check for maximum value of coherence score and minimum value for perplexity, if the graph is non decreasing we will look for the value from where the slope become constant.
The value we got from graph will be our number of topics and then we will generate keywords and topic would be inferred from it.



 

## Installation
--------------------------------------------------------------------------------------------------------------------------------
[(Back to top)](#list-of-contents)

Following Python Libraries need to be installed for the successful completion of project.
- [Librosa](https://librosa.github.io/librosa/)
- [Pandas](https://pandas.pydata.org/)
- [Numpy](https://numpy.org/)
- [speechRecognition](https://pypi.org/project/SpeechRecognition/)
- [PyAudio](https://pypi.org/project/PyAudio/)
- [matplotlib](https://matplotlib.org/)
- [goslate](https://pypi.org/project/goslate/)
- [SciPy](https://www.scipy.org/)
- [gensim](https://pypi.org/project/gensim/)
- [nltk](https://www.nltk.org/)
- [re](https://docs.python.org/3/library/re.html)
- [pprint](https://docs.python.org/2/library/pprint.html)
- [spaCy](https://spacy.io/)


Install above required packages using pip or any other method.

Note : You can simply use Google Colab which already has configured environment!

## Running

- calculating perplexity and coherence values

![img](https://imgur.com/kpv1s3C.png)

- generating keywords
![img](https://imgur.com/mD2n2Gb.png)

- how to infer topics from keywords 
![img](https://imgur.com/t90WmgP.png)



