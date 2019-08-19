# Language as a Tree

The material in this directory explains how syntactic trees are used in NLP, teaches algorithms of dependency parsing, and shows how to build a simple dependency parser for the Estonian language.

The code is presented using iPython. You can either use the Colab environment to run the code in the cloud or install the needed software on your computer and run the code locally. See below for details.

## To run in Colab

How to run code in Colab:
- open the notebook via [this link](https://colab.research.google.com/drive/17f0sDK_HtaMNYE2TD0bsK851gF-uiot-#scrollTo=20I7QKaxu6Wb&forceEdit=true&offline=true&sandboxMode=true)
- press Shift+Enter to run a block of code
- on the first run, you'll see a warning from Google; press "Run anyway"

## To run locally

Clone this repository.

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

## To follow without running

Simply open the jupyter notebook in your browser.

If you get an error message _Sorry, something went wrong. Reload?_ while loading a notebook in your browser, try opening the notebook with the help of https://nbviewer.jupyter.org.
