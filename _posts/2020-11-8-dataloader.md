---
layout: post
title: Dataset and Dataloader
subtitle: PyTorch's Dataset and Dataloader
tags: [PyTorch]
comments: true
---

## Dataset
PyTorch supports two different types of datasets.  

**map-style datasets**
* Represents a map from (possibly non-integral) indices/keys to data samples.
* Implements the __getitem__() and __len__() protocols, and 
* When accessed with dataset[idx], could read the idx-th image and its corresponding label from a folder on the disk.

**iterable-style datasets**
* Represents an iterable over data samples.
* Implements the __iter__() protocol, and 
* This type of datasets is particularly suitable for cases where random reads are expensive or even improbable, and where the batch size depends on the fetched data.


Reference
[link](https://pytorch.org/docs/stable/data.html)
