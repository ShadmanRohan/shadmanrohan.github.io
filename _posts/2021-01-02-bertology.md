---
layout: post
title: Sample blog post
subtitle: Each post also has a subtitle
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---

> <em>paper: <https://arxiv.org/pdf/1502.03167.pdf%27></em>

## Model
BERT is a stack of Transformer
encoder layers (Vaswani et al., 2017) which consist
of multiple self-attention "heads". For every input
token in a sequence, each head computes key, value
and query vectors, used to create a weighted representation. The outputs of all heads in the same layer
are combined and run through a fully-connected
layer. Each layer is wrapped with a skip connection
and followed by layer normalization.

## Training
The conventional workflow for BERT consists of two stages: pre-training and fine-tuning. Pretraining uses two self-supervised tasks: masked language modeling (MLM, prediction of randomly masked input tokens) and next sentence prediction
(NSP, predicting if two input sentences are adjacent
to each other). In fine-tuning for downstream applications, one or more fully-connected layers are
typically added on top of the final encoder layer.

## Bert's internal knowledgebase
1. Syntactic knowledge
* BERT representations are hierarchical rather than linear
* BERT embeddings encode information about parts of speech, syntactic chunks and roles.
* Syntactic information can be recovered from BERT token representations
* BERT "naturally" learns some syntactic information, although it is not very similar to linguistic annotated resources.
* BERT takes subject-predicate agreement into account when performing the cloze task.
* Bert is better able to detect the presence of NPIs (e.g. "ever") and the words that allow their use(e.g "whether") than scope violations.
* Bert does not "understand" negation and is insensitive to malformed input.
* BERT’s syntactic knowledge is incomplete, or it does not need to rely on it for solving its tasks.
2. Semantic knowledge
3. World knowledge

## Limitations


## Fine-tuning of BERT
1. Taking more layers into account
2. Two-stage fine-tuning
3. Adversarial token perturbations
4. Adversarial regularization
5. Mixout regularization
