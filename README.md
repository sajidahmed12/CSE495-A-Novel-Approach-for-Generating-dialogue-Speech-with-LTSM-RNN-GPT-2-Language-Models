# A-Novel-Approach-for-Generating-dialogue-Speech-with-LTSM-RNN-GPT-2-Language-Models
Analysis of GoT dialogues using NLP techniques. 

The main question we would like to answear is how dialogues relate characters in GoT series, and what we can learn from those relationships and weather or not using a neural network to generate dialogues will be a viable thing to do. 

# Required Libraries to install

This project requires **Python 3.6+** and the following Python libraries installed:

- [numpy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [seaborn](https://seaborn.pydata.org/)
- [fastai](https://github.com/fastai/fastai)
- [networkx](https://networkx.github.io/documentation/stable/install.html)
- [nltk](https://www.nltk.org/install.html)
- [genism](https://radimrehurek.com/gensim/install.html)

# Dataset

We have obtained the raw dialogues from [Genius.com](https://genius.com/artists/Game-of-thrones), these were trancribed by volunteers, so not all
seasons are there and of course there will be some mistakes, but is the best there is.

All the csv files we have used are available [here](https://github.com/sajidahmed12/CSE495-A-Novel-Approach-for-Generating-dialogue-Speech-with-LTSM-RNN-GPT-2-Language-Models/tree/main/Game-of-thrones-analysis/CSV), and you can find how we have transformed the raw text into a more useful csv in the 
[Final_Pipeline](https://github.com/sajidahmed12/CSE495-A-Novel-Approach-for-Generating-dialogue-Speech-with-LTSM-RNN-GPT-2-Language-Models/tree/main/Game-of-thrones-analysis/Final_Pipeline.ipynb) notebook.

## File description.

[Final_Pipeline](https://github.com/sajidahmed12/CSE495-A-Novel-Approach-for-Generating-dialogue-Speech-with-LTSM-RNN-GPT-2-Language-Models/tree/main/Game-of-thrones-analysis/Final_Pipeline.ipynb): The whole process from data preparation and analysis to modeling and scoring.

[GoT dialogue generator](https://github.com/sajidahmed12/CSE495-A-Novel-Approach-for-Generating-dialogue-Speech-with-LTSM-RNN-GPT-2-Language-Models/tree/main/Game-of-thrones-analysis/GoT%20dialogue%20generator.ipynb): Using a pre trained model to generate random GoT dialogues. 

[GoT](https://github.com/sajidahmed12/CSE495-A-Novel-Approach-for-Generating-dialogue-Speech-with-LTSM-RNN-GPT-2-Language-Models/tree/main/Game-of-thrones-analysis/GoT): All raw form of chapter scripts obtained from [Genius.com](https://genius.com/artists/Game-of-thrones).

[CSV](https://github.com/sajidahmed12/CSE495-A-Novel-Approach-for-Generating-dialogue-Speech-with-LTSM-RNN-GPT-2-Language-Models/blob/main/Game-of-thrones-analysis/CSV): Three CSV files, if you want to follow all the data cleaning we did it foryou if need. 4 columns they contain: Character, dialogue, season and chapter. The rows vary from file to file but around 14K. 


## Network Graph

We have also created a network graph using the character interaction obtained from the dialogues.
<p align="left">
  <img src=doc/graph.JPG>  
</p>


## Dialogue generation.

All the text generation happens in this [notebook](https://github.com/sajidahmed12/CSE495-A-Novel-Approach-for-Generating-dialogue-Speech-with-LTSM-RNN-GPT-2-Language-Models/blob/main/Game-of-thrones-analysis/GoT%20dialogue%20generator.ipynb)

# Model Training 
## To the Ipython notebook to "RUN ALL models test and train"

## To Run The Source .py or ipynb Files Follow the instructions written in runmeforallwork.ipynb and then we can easily test and also train our 3 implementions Of Our NLP Project. 

# GPT-2 language Model Dialogue Generation Performace 

* Perplexity 
<p align="left">
  <img src=doc/LaTexSourceFiles/images/GPTPerp.png>  
</p>

* Loss 
<p align="left">
  <img src=doc/LaTexSourceFiles/images/GPTLoss.png>  
</p>

# Some Generated Dialogue Samples 

<p align="left">
  <img src=doc/speech\sample\100.JPG>  
</p>

<p align="left">
  <img src=doc/speech\sample\50.JPG>  
</p>

So What we have done so far !! 
* 1. LSTM Model
* 2. RNN seq-to-seq Model
* 3. GPT-2 language Model based Dialogue generator


# Submitted by group Members

- [Md.Sajid Ahmed -1610364042](https://github.com/sajidahmed12)
- [Zahin Akram -1610618042](https://github.com/ZahinAkram)
- [Arifuzzaman Arman -1610551042]
- [Md Rakib Imtiaz -1610294042]

## Licensing, Authors, Acknowledgements
I have to give credit to all the volunteers at Genius for transcribing the dialogues as well as to [Paras Chopra](https://towardsdatascience.com/generating-new-ideas-for-machine-learning-projects-through-machine-learning-ce3fee50ec2) and [Daniel E. Licht](https://lichtphyz.github.io/) whose work is the base of this project. Apart from that feel free to use the code and files as you wish.

