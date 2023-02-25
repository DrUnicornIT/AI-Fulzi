---
layout: page
title: Word Embeddings
permalink: ainlp/word-embedding
---

## Overview

- (Nikolov et al, 2013) [Distributed Representation of Words and Phrases and their Compositionality](https://proceedings.neurips.cc/paper/2013/file/9aa42b31882ec039965f3c4923ce901b-Paper.pdf)
- (Baroni et al, 2014) [Don't count, predict! A systematic comparison of context-counting vs context-predicting semantic vectors](https://aclanthology.org/P14-1023.pdf)

## Distributed representations of words

Using in a vector space help learning algorithms to achieve better performance in natural language processing (NLP) tasks by grouping similar words.

The word representations computed using neural networks are very interesting because the learned vectors explicily encode many linguistic regularities and patterns.

For example, the result of a vector calculation:

> Vec("Paris") - Vec("France") + vec("VietNam") is closer to vec("HaNoi")

Linguistic regularities  
![alt text]({{ site.github.url }}/assets/img/Linguistic regularities.png "Linguistic regularities")

## Distributional hypothesis

Distributiona hypothesis: words that occur in similar cotexts tend to have similar meanings
J.R.Firth 1957

- You shall know a word by the company it keeps
- One of the most successful ideas of modern statistical NLP

## Lantent Semantic Analysis

([SVD-based methods](https://www.sciencedirect.com/topics/engineering/singular-value-decomposition))
LSA is a technique in NLP, in particular distributional semantics, of analyzing relationships between a set of documents and the terms they contain by producing a set of concepts related to the docments and terms. LSA assumes that words that are close in meaning will occur in similar pieces of text (Distributional hypothesis) - _wikikipedia_

![alt text]({{ site.github.url }}/assets/img/LSA.png "LSA")

## Collobert & Weston vectors

**Idea:** a word and its context is a positive training sample; a random word in that sample context gives a negative training sample:

> Score(cat chills on a mat) > Score(cat chills Ohio a mat)

## The Skip-Gram Model

- The idea: we want to use words to predict their context words.
- Context: a fixed windown of size 2m

![alt text]({{ site.github.url }}/assets/img/PSkipgram.png "PSkipgram")

More formally, given a sequence of training words, the objective of the [Skip-gream model](https://aegis4048.github.io/demystifying_neural_network_in_skip_gram_language_modeling) is

$$\frac{1}{T} \sum_{t=1}^{T} \sum_{-c\leq j \leq c, j \neq 0} log P(w_{t+j}|w_t)$$

## How to define $P(w_{t+j}|w_t)$

We have two sets of vectors for each word in the vocabulary

- $$u_i \in R^d$$: embedding for center word i
- $$v_{i'} \in R^d$$: embedding for context word i'

Use inner product $u_i . v_{i'}$ to measure how likely word i appears with context word i', the larger the better
$$P(w_{t+j}|w_t) = \frac{exp(u_{w_t}.v_{w_{t+j}})}{\sum{k \in V}exp(exp(u_{w_t}.v_{k})}$$

## Hierarchical softmax

![alt text]({{ site.github.url }}/assets/img/Hierarchical softmax.png "Hierarchical softmax")

## Negative sampling & NCE

An alternative to the hierarchical softmax is Noise Contrastive Estimation (NCE), NCE posits that a good model should be able to differentiate data from noise by means of logistic regression.

## Subsampling of Frequent Words

In very large corpora, the most frequent words can easily occur hundreds of millions of times (e.g., “in”, “the”, and “a”). Such words usually provide less information value than the rare words. For example, while the Skip-gram model benefits from observing the co-occurrences of “France” and “Paris”, it benefits much less from observing the frequent co-occurrences of “France” and “the”, as nearly every word co-occurs frequently within a sentence with “the”. This idea can also be applied in the opposite direction; the vector representations of frequent words do not change significantly after training on several million examples.

Probability of discarding a word:

$$P(w_i) = 1 - \sqrt{\frac{t}{f(w_i)}} (t=1e-5)$$

## Learning phrases

"New York Time" != "New" + "York" + "Times"  
"Air Canada" != "Air" + "Canada"

A simple data-drive approach to celect pharases:
$$score(w_i, w_j) = \frac{count(w_iw_j)-\delta}{count(w_i)\times count(w_j)}$$
![[Learning phrases.png]]

## Don't count, predict

- A systematic comparative evaluation of count and predict vectors
- Main result: predict vectors >> count vectors

## Count vs predict models

- "Count" models: collect raw co-occurrence counts in a corpus, and transform them into vectors with dimensionality reduction (and reweighting)
- "Predict" models: estimate the word vectors directly by maximizing the probability of the contexts in which the word in observed in the corpus

## Semantic relatedness

Similarity vs relatedness:

- "car" vs "vechicle"
- "car" vs "journey"

Compare thecorrelation between the average scores that human subjects assigned to the pairs and cosine similarity between corresponding vectors

## Synonym detection

TOEFL test

- levied: _imposed_, believed, requested, correlated

## Concept categorization

- "elephants" -> "mammal

## Selectional preferences

Paper: [Selectional Preferences for Semantic Role Classification](https://aclanthology.org/J13-3006.pdf)

Verb-noun pairs
Sample:

- Smith was assassinated in Texas
- Smith was assassinated in December
