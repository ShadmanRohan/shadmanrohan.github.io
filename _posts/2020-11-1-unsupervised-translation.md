---
layout: post
title: Unsupervised Machine Translation Using Monolingual Corpora Only!
subtitle: Some random notes from the paper
thumbnail-img: /assets/img/monocorp.png
tags: [PaperReview]
---

### Paper Review!
My actual journey into deeplearning began with this paper. Although I could not reproduce it but I learnt many important techniques from this gem.

### BackTranslation
This was the most interesting. The prediction from the model on the target side was used as source sentence to predict the original sentence. I found this super interesting!

### Alignment of Monolingual word embedding space 
> [https://arxiv.org/abs/1710.04087]
See the FastText Library for more

### Alignment of Sentence Meaning space
The encoder acts as the generator while the discriminator tries to identify the language of source sentence. When the discriminator makes random predictions, it signifies that the sentences with the same meaning are getting mapped into the same location.

### Intuition 
The idea behind the algorithm is that as long as the initial model retains at least some information of the input sentence, the encoder will map such translation to vectors in the latent space that also correspond to a cleaner version of the input because the encoder is trained to denoise. At the same time, the decoder is trained to predict noiseless outputs, given noisy features. Putting these two things together will produce less noisy translations, which will enable better back-translations at the next iteration, and so on so forth.

> paper <https://arxiv.org/abs/1711.00043>  

> useful link <https://yashuseth.blog/2019/03/03/how-can-unsupervised-neural-machine-translation-work/#:~:text=Unsupervised%20Machine%20Translation%20requires%20only,MT%20systems%20makes%20intuitive%20sense.>
