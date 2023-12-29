# Aspect Based Sentiment Analysis

## Team Members
- Anushka Jain
- Tanish Taneja

## Project Description
This project was made as part of our final project for the course, Statistical Methods in AI, offered at IIIT Hyderabad. The project aims at developing a heirarchical bi-LSTM model which performs aspect based sentiment analysis on reviews provided by users for different products across different languages. We have also developed CNN and LSTM models for comparison along with the H-LSTM. Currently, the project is only functional for the English language.

## Topic : <b>A hierarchical model of reviews for aspect based sentiment analysis</b>
### Important Files
- [documents/main-paper.pdf](https://github.com/anushkaj1/aspect-based-sentiment-analysis/blob/main/documents/main-paper.pdf) : The paper being implemented in the project.
<!-- - [documents/smai-project-proposal.pdf](https://github.com/Statistical-Methods-in-AI-Monsoon-2023/project-huh-lmao/blob/main/documents/smai-project-proposal.pdf) : An initial proposal and deliverables to complete the project. -->
- [documents/datasets-paper.pdf](https://github.com/anushkaj1/aspect-based-sentiment-analysis/blob/main/documents/datasets-paper.pdf) : Contains the documentation of SemEval 2016 Task 5 and other useful information regarding the problem 
- [README.md](https://github.com/anushkaj1/aspect-based-sentiment-analysis/blob/main/README.md) : The documentation of the repository.
- [smai-project-environment.yml](https://github.com/anushkaj1/aspect-based-sentiment-analysis/blob/main/smai-project-environment.yml) : Contains a virtual conda env which contains all the required libraries used.

### Code
#### preprocessing.ipynb
- Preprocesses the XML data and saves it in the form of CSV files in `preprocessed_datasets`. 
- This is done to provide an easier method to read the data manually by users. All models are coded to run using XML files, the original format in which data is provided.
#### embeddings.ipynb
- Embeds the provided dataset using GloVe embeddings which can be used for further computation.
#### cnn.ipynb
- Contains implementation of 2 CNN Models (Aspect Category Detection and Sentiment Polarity).
#### lstm.ipynb
- Contains implementation of 2 LSTM Models (Aspect Category Detection and Sentiment Polarity).
#### H-lstm.ipynb
- Contains implementation of the HLSTM model.
- In this model, first the input sentences are sent through an LSTM model. The outputs of this model are sent through another LSTM, this time at the review level instead of sentence-level and the output obtained gives the final sentiment of the model.
