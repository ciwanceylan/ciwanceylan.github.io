---
layout: page
permalink: /mscthesisproposals/
title: master thesis proposals
description: 
years: [2020]
nav: false
---

## 2020

### Large scale / attributed generation of complex networks

**Start date:** Autumn 2020


Generative models are defined by the possibility to generate new samples after the model has been trained on some dataset. Recently, much progress has been made in training generative models for image data (e.g. using [generative adversarial networks (GANs)](https://en.wikipedia.org/wiki/Generative_adversarial_network), [variational autoencoders (VAEs)](https://towardsdatascience.com/understanding-variational-autoencoders-vaes-f70510919f73) and [autoregressive models](https://towardsdatascience.com/autoregressive-models-pixelcnn-e30734ede0c1)). The fact that the performance of these models have not yet extended to other types of data, e.g. text, structured data and complex networks, indicate that they are largely reliant of the underlying model, i.e. the powerful convolutional neural network for images. While some progress have been made in recent years, it is important to explore new ways and models to be leveraged for these other data types. For this proposal, graphs and complex networks are in focus.

Generative models for networks have a long history going back to random graph models such as the [Erdős–Rényi model](https://en.wikipedia.org/wiki/Erd%C5%91s%E2%80%93R%C3%A9nyi_model) studied in graph theory. 
In this vein of "classical" generative models for networks we find widely used models such as [R-MAT](https://www.cs.cmu.edu/~christos/PUBLICATIONS/siam04.pdf), the [stochastic block model(SBM)](http://tuvalu.santafe.edu/~aaronc/courses/5352/fall2013/csci5352_2013_L16.pdf) with extensions, e.g. [degree-corrected](https://arxiv.org/abs/1008.3926) and the [exponential random graph model (ERGM)](https://www.jstor.org/stable/2287037).
These models are still being worked on and extended today, e.g. [Bayesian SBMs](https://arxiv.org/pdf/1705.10225.pdf), [improved inference for ERGM](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0227804) and [general implementation improvements](https://ieeexplore.ieee.org/document/7877110). 

Recently researches have been looking to more "modern" graph generation models by trying to leverage deep learning techniques. Typically a GAN, VAE or auto-regressive objective is used and combined with either a recurrent neural network, e.g. 
[GraphRNN](https://arxiv.org/abs/1802.08773) and
[NetGAN](https://arxiv.org/abs/1803.00816),
or a [graph convolutional neural network](https://arxiv.org/abs/1609.02907), e.g. 
[Variational Graph Auto-Encoders](https://arxiv.org/pdf/1611.07308.pdf),
[Graphite](http://arxiv.org/abs/1803.10459) and
[GRAN](https://arxiv.org/abs/1910.00760).
But other types of models are also possible, such as [Misc-GAN](https://www.frontiersin.org/articles/10.3389/fdata.2019.00003/full) which uses tools from the field of [graph processing](https://www.macalester.edu/~dshuman1/Papers/Journal/Shuman_et_al_SPM_2013.pdf).

While these modern models are able to model much more complex networks in theory, they are still not fully mature. They don't scale to as large networks as the classical models and they are often not implemented to account for node and edge attributes or directed graphs. It is in these area where we hope to make progress by proposing two different master's thesis topics.

The two topics we are offering are:
1. Attempting to scale up neural network based network generation models to work for very large but sparse graphs. The main idea is to use some hierarchical structure, getting inspiration from classical graph generation models or possibly include them as a step in a pipeline.
2. Extend a modern model to account for node attributes, weighted graphs, time-evolving graphs or directed graphs. All of these are possible directions and we will have to discuss what feel the most reasonable within the time scope of the thesis.

#### Requirements
* Background in machine learning or computer science.
* Good implementation skills in Python using numpy, scipy etc..
* Previous experience with Pytorch and/or graph processing library is a big plus.
* For project 1 it is important that you feel comfortable with implementation as we will want to work with quite large datasets at some point during the project.
* Project 2 could be treated more theoretically in which case you should be comfortable with mathematical exploration.

