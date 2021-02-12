---
layout: post
title: OCR
gh-badge: [ocr]

---

The four stages derived from existing STR models are as
follows:
1. Transformation (Trans.) normalizes the input text image using the Spatial Transformer Network (STN [12]) to ease downstream stages.
2. Feature extraction (Feat.) maps the input image to a representation that focuses on the attributes relevant for character recognition, while suppressing irrelevant features such as font, color, size, and background.
3. Sequence modeling (Seq.) captures the contextual information within a sequence of characters for the next stage to predict each character more robustly, rather than doing it independently.
4. Prediction (Pred.) estimates the output character sequence from the identified features of an image.

### CRNN
![Crepe](https://github.com/ShadmanRohan/shadmanrohan.github.io/blob/master/assets/img/ocr.jpg)

