# BertPT and AlbertPT
Pre-trained **Portuguese** versions of Bert and Albert

## Introduction
*BERT*, Bidirectional Encoder Representations from Transformers is a method of pre-training language models.

The official models released were pre-trained in English, Chinese and a Multilingual that was trained combining 104 languages.

In this repository, we release a base version that was trained using **Portuguese** version of Wikipedia.

## Why Pre-training?
When training for a NLP task, a model must learn to extract features from training data and build a good representation of the language.
Often, there is not enough data available for the model to learn to understand the text and to solve the problem.
In these situations, pre-training helps because the model is already able to generate good representations that can be used to solve a great variety of NLP problems.
The pre-training is an unsupervised and quite expensive task.

After the pre-training, the model can be fine-tuned (trained) for a specific task in just a few minutes. 

## Pre-Training Corpus
- [Wikipedia](https://dumps.wikimedia.org/backup-index.html)
- [CHAVE](https://www.linguateca.pt/CHAVE/)
- [Open Subtitles](http://opus.nlpl.eu/OpenSubtitles-v2016.php)
- [EuroParl](http://opus.nlpl.eu/Europarl.php)
- [Abstracts from Dominio Publico](http://www.dominiopublico.gov.br/pesquisa/PesquisaObraForm.jsp)

Abstracts already assembled [teses](https://drive.google.com/open?id=1faI_PVQiiWvP0qK9UQGq7D78KKqs8t1H)

## Models
Both models are able to produce very good results in NLP tasks.
Bert base model has 110M parameters, while Albert base model has only 12M. 

- [albert_cased_L-12_H-768_A-12](https://drive.google.com/open?id=1GUveRMJyBJmDmCWnnz7OrdEZsGtKFQ6S)
- [bert_cased_L-12_H-768_A-12](https://drive.google.com/open?id=1qQ0WL9GGg8P1g8eOOxW8Ts9GXQA4IoEo)

## Evaluation
See our paper for a comprehensive evaluation (To Be Released).

Our experiments suggest similar performance. 
We also compare the these models to the official Bert Multilingual model.

## Usage
It is possible to find usage instructions in the [Oficial Bert Repository](https://github.com/google-research/bert)

## References
- [Bert](https://github.com/google-research/bert): Pre-training of Deep Bidirectional Transformers for Language Understanding 
- [Albert](https://github.com/google-research/albert): A Lite Bert for Self-Supervised Learning of Language Representations
 


