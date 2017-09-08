---
layout: post
title: Overview
---
In this paper, we make a simple observation that questions about images often contain premises - objects and relationships implied by the question - and that reasoning about premises can help Visual Question Answering (VQA) models respond more intelligently to irrelevant or previously unseen questions. 

When presented with a question that is irrelevant to an image, state-of-the-art VQA models will still answer purely based on learned language biases, resulting in non-sensical or even misleading answers. We note that a visual question is irrelevant to an image if at least one of its premises is false (i.e. not depicted in the image). We leverage this observation to construct a dataset for Question Relevance Prediction and Explanation (QRPE) by searching for false premises. 

We train novel question relevance detection models and show that models that reason about premises consistently outperform models that do not. We also find that forcing standard VQA models to reason about premises during training can lead to improvements on tasks requiring compositional reasoning.

![_config.yml]({{ site.baseurl }}/images/teaser.png)
Questions asked about images often contain ‘premises’ that imply visual semantics. From the above question, we can infer that a relevant image must contain a man, a racket, and that the man must be holding the racket. We extract these premises from visually grounded questions and use them to construct a new dataset and models for question relevance prediction. We also find that augmenting standard VQA training with simple premise-based questions results in improvements on tasks requiring compositional reasoning.

## Authors

[Aroma Mahendru](https://computing.ece.vt.edu/~aroma/)\*, [Viraj Prabhu](https://virajprabhu.github.io)\*, [Akrit Mohapatra](https://computing.ece.vt.edu/~akrit/)\*, [Dhruv Batra](https://www.cc.gatech.edu/~dbatra/index.html), [Stefan Lee](https://www.cc.gatech.edu/~slee3191/index.html) 

(* = equal contribution)