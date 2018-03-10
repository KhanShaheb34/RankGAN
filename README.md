# RankGAN

## Requirements: 
* **Tensorflow r1.6.0**
* Python 3.x
* CUDA 9.0 (For GPU)

## Introduction
Apply Generative Adversarial Nets to generating sequences of discrete tokens with optimization via replacing the discriminator with a ranker.

The previous research paper [SeqGAN: Sequence Generative Adversarial Nets with Policy Gradient](http://arxiv.org/abs/1609.05473) has been accepted at the Thirty-First AAAI Conference on Artificial Intelligence (AAAI-17).

The research paper [Adversarial Ranking for Language Generation](https://papers.nips.cc/paper/6908-adversarial-ranking-for-language-generation.pdf) has been accepted at 31st Conference on Neural Information Processing Systems (NIPS 2017).

We reproduce example codes to repeat the synthetic data experiments with oracle evaluation mechanisms.
To run the experiment with default parameters:
```
$ python sequence_gan.py
```
You can change the all the parameters in `sequence_gan.py`.

The experiment has two stages. In the first stage, use the positive data provided by the oracle model and Maximum Likelihood Estimation to perform supervise learning. In the second stage, use adversarial training to improve the generator.


Note: this code is based on the [previous work by ofirnachum](https://github.com/ofirnachum/sequence_gan) and [SeqGAN](https://github.com/LantaoYu/SeqGAN) . 
