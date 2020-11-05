---
layout: post
title: Normalization in Deep Learning
subtitle: Only the techniques I have encountered... there are many more!
tags: [DeepLearning]
comments: true
---

### Batch Normalization<br>*paper: <https://arxiv.org/pdf/1502.03167.pdf%27>*

Training Deep Neural Networks is complicated by the fact that the distribution of each layer’s inputs changes during training, as the parameters of the previous layers change. This slows down the training by requiring lower learning rates and careful parameter initialization, and makes it notoriously hard to train models with saturating nonlinearities. We refer to this phenomenon as internal covariate shift, and address the problem by normalizing layer inputs. Our method draws its strength from making normalization a part of the model architecture and performing the normalization for each training mini-batch. Batch Normalization allows us to use much higher learning rates and be less careful about initialization. It also acts as a regularizer, in some cases eliminating the need for Dropout.

### Layer Normalization


### Weight Normalization


### Group Normalization


### Instance Normalization
