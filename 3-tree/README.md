# Language as a Tree

The material in this directory explains how syntactic trees are used in NLP, teaches algorithms of dependency parsing, and shows how to build a simple dependency parser for the Estonian language.

The code is presented using iPython. You can either use the Colab environment to run the code in the cloud or install the needed software on your computer and run the code locally. See below for details.

## To run in Colab

How to run code in Colab:
- open the notebook via [this link]()
- press Shift+Enter to run a block of code
- on the first run, you'll see a warning from Google; press "Run anyway"

## To run locally

Clone the repository.

Clone [the repository with Estonian Universal Dependencies](https://github.com/UniversalDependencies/UD_Estonian-EDT).

Make sure you have the following installed:
- Python 3
- scikit-learn>=0.20.3, numpy>=1.16.1, scipy>=1.3.0
```
pip install -U scikit-learn
```
- connll
```
pip install conllu
```
- jupyter
```
pip install jupyter
```

How to run code locally:
- run `jupyter notebook` in Terminal from the repository folder
- press Shift+Enter to run a block of code
