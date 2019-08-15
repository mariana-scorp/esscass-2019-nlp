# Feature Engineering for Natural Language Processing

The material in this directory showcases how to extract linguistic features from text using the spaCy library, how to encode these features using sklearn, and how to build a simple classifier to detect incorrect adjective/adverb usage with verbs.

The code is presented using iPython. You can either use the Colab environment to run the code in the cloud or install the needed software on your computer and run the code locally. See below for details.

## To run in Colab

Links in Colab:
* [feature-encoding.ipynb](https://colab.research.google.com/drive/1vn-2t-PAgAl4eD7DP7ywsWV1kHEqOBnK#scrollTo=_qJn_sD4ii2k&forceEdit=true&offline=true&sandboxMode=true)
* [adjective-vs-adverb.ipynb](https://colab.research.google.com/drive/1MU3Z0mf8pAfM7bITKzZeJZTTlzBj1co4#forceEdit=true&offline=true&sandboxMode=true&scrollTo=UBXPt9RmxIpm)

How to run code in Colab:
- open the notebook via the link (see above)
- press Shift+Enter to run a block of code
- on the first run, you'll see a warning from Google; press "Run anyway"

## To run locally

Clone the repository.

Make sure you have the following installed:
- Python 3
- spacy>=2.1.8
```
pip install -U spacy
```
- spacy models for the English language (here en-core-web-md=2.1.0; with other versions the results may differ)
```
python -m spacy download en_core_web_md
```
- scikit-learn>=0.20.3, numpy>=1.16.1, scipy>=1.3.0
```
pip install -U scikit-learn
```
- jupyter
```
pip install jupyter
```

How to run code locally:
- run `jupyter notebook` in Terminal from the repository folder
- press Shift+Enter to run a block of code

## Contents

The [data](data/) folder contains:
- lists of adjectives and adverbs extracted from the English Wiktionary (see http://dumps.wikimedia.your.org/enwiki/20180401/)
- a data set of 20,000 sentences extracted from [The Blog Authorship Corpus](http://u.cs.biu.ac.il/~koppel/BlogCorpus.htm)

The [aux](aux/) folder contains a script for extracting the data set from [The Blog Authorship Corpus](http://u.cs.biu.ac.il/~koppel/BlogCorpus.htm).

[feature-encoding.ipynb](feature-encoding.ipynb) contains a simple example of feature extraction with spaCy and feature encoding with sklearn.

[adjective-vs-adverb.ipynb](adjective-vs-adverb.ipynb) contains a simple solution for the task of correcting confused adjectives and adverbs:
- How do we change adjectives to adverbs and vice versa?
- What features distinguish adjectives from adverbs?
- Where do we get data?
- How do we use the classifier for error correction?
