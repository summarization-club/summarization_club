# Cryptonews headlines generator

Idea: Can we generate good news headline from text?

Target Dataset: https://www.kaggle.com/kashnitsky/news-about-major-cryptocurrencies-20132018-40k

Metrics: ROUGE-1, ROUGE-2, ROUGE-L, average

## Baseline 
https://www.kaggle.com/kashnitsky/cryptonews-headline-generation-first-30-words by @yorko - which metrics has headline consisting of the first 30 words?


## Baselines to build:
* first 30 words (16.6%, 4.7%, 15.7%, 12.3%)
* find patterns by eyes
* unsupervised methods - TextRank
* seq2seq, input - all text (OpenNMT)
* seq2seq, input - first 1-3 sentenses (OpenNMT)
* simple transformer (OpenNMT)

## Tools and experiments

* try to apply BART
* pretrain on external dataset - NYT Annotated (https://catalog.ldc.upenn.edu/LDC2008T19)
* gather more data (dataset we have was gathered in 2018)
* try to use PEGASUS
* try to use T5
* try some custom architectures from FairSeq (https://github.com/pytorch/fairseq)"