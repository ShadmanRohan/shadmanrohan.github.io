---
layout: post
title: Neural approaches to Translation 
subtitle: An overview of important concepts for neural machine translation
tags: [nlp, nmt]
---

### Background
* rule based -> statistical -> neural
* a sequence to sequence problem.


The latest neural network based approaches mainly involves variants of the transformer or the recurrent models. While the recurrent model is more robust, the transformer based approach produces better results by consuming more data in a paralellized manner. I will be mostly covering the recurrent models for machine translation here.   

### Language Models
Conditional language modelling is currently the most popular machine translation technique. It involves calculating the probability for each term in the sequence conditioned on the input sentence and previous outputs.

$$
P(y | x)=P\left(y_{1} | x\right) P\left(y_{2} | y_{1}, x\right) P\left(y_{3} | y_{1}, y_{2}, x\right) \ldots P\left(y_{T} | y_{1}, \ldots, y_{T-1}, x\right)
$$

### Handling Unknown Words
* Assume closed Vocabulary
* Interpolate with an unknown words distribution
* Add an &lt;p&gt; unk &lt;/p&gt; word
