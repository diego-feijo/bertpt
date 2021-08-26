# BertPT and AlbertPT
Pre-trained **Portuguese** versions of Bert and Albert. This models were pre-trained and evaluated in our public acessible paper (https://arxiv.org/abs/2007.09757).

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

## Auxiliary Datasets
- Assembled abstracts [teses](https://drive.google.com/open?id=1faI_PVQiiWvP0qK9UQGq7D78KKqs8t1H)
- Polarity Sentiment Tweets [polarity_sentiment_tweets](https://drive.google.com/open?id=1-VvfOaph71Dlq6ZdVGQP7bAnmy33QIoj)

## Models
Both models are able to produce very good results in NLP tasks.
Bert base model has 110M parameters, while Albert base model has only 12M. 

- [albert_cased_L-12_H-768_A-12](https://drive.google.com/open?id=1GUveRMJyBJmDmCWnnz7OrdEZsGtKFQ6S)
- [bert_cased_L-12_H-768_A-12](https://drive.google.com/open?id=1qQ0WL9GGg8P1g8eOOxW8Ts9GXQA4IoEo)

## Evaluation
See our paper(https://arxiv.org/abs/2007.09757) for a comprehensive evaluation.

Our experiments suggest similar performance. 
We also compare the these models to the official Bert Multilingual model.

## Usage
We released two Colab notebooks to show how to use it:
1. [Pre-training ALBERT from Wikipedia using TPU](Pre_training_ALBERT_from_Wikipedia_using_TPU.ipynb)
2. [Fine-tuning ALBERT for Fake News Detection](Fine_tuning_ALBERT_for_Fake_News_Detection.ipynb)

The first kernel uses Wikipedia (it can use any language) to train a Base ALBERT model.
The second kernel uses the model trained on step one to fine-tune for the task of predicting Fake News (in Portuguese). This model achieves state-of-the-art results after fine-tuning for less than five minutes.

## References
- [Bert](https://github.com/google-research/bert): Pre-training of Deep Bidirectional Transformers for Language Understanding 
- [Albert](https://github.com/google-research/albert): A Lite Bert for Self-Supervised Learning of Language Representations
 
## Citation
```bibtex
@article{feijo2020mono,
  title={Mono vs Multilingual Transformer-based Models: a Comparison across Several Language Tasks},
  author={Feijo, Diego de Vargas and Moreira, Viviane Pereira},
  journal={arXiv preprint arXiv:2007.09757},
  year={2020},
  url={https://arxiv.org/abs/2007.09757}
}
```

