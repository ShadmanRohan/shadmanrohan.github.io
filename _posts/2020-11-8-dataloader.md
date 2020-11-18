---
layout: post
title: Dataset and Dataloader
subtitle: PyTorch's Dataset and Dataloader
tags: [PyTorch]
comments: true
---

[link](https://pytorch.org/docs/stable/data.html)

PyTorch supports two different types of datasets.  
**map-style datasets**
* Represents a map from (possibly non-integral) indices/keys to data samples.
* Implements the __getitem__() and __len__() protocols, and 
* when accessed with dataset[idx], could read the idx-th image and its corresponding label from a folder on the disk.


**iterable-style datasets**

