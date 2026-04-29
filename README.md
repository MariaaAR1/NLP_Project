# Central Bank Communication as Alternative Data

This repository contains the code and report for an NLP project on topic modeling of BIS central bank speeches.

## Project objective

The project studies whether unsupervised NLP methods can extract interpretable macro-financial topics from central bank speeches and how these topics evolve over time.

## Dataset

The dataset is the BIS central bank speeches dataset from Hugging Face:
`samchain/bis_central_bank_speeches`.

## Notebooks

1. `01_EDA.ipynb`: exploratory data analysis.
2. `02_Preprocessing.ipynb`: text cleaning, lemmatization, filtering and construction of the final corpus.
3. `03_TFIDF_NMF.ipynb`: TF-IDF representation and NMF topic modeling.
4. `04_LDA.ipynb`: count-based LDA topic modeling.
5. `05_BERTopic.ipynb`: embedding-based BERTopic analysis.

## Main methods

- TF-IDF + NMF
- CountVectorizer + LDA
- Sentence embeddings + BERTopic

## Main conclusion

NMF provides the clearest macro-financial topics. LDA confirms several broad themes but produces more diffuse topics. BERTopic reveals that the corpus is also strongly structured by institutional and geographical communication patterns.
