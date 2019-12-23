---
layout: default
title: Deep Learning
parent: Artificial Intelligence
nav_order: 1
---
# Atomospheric Deep Learning
[cloud segmentation](https://medium.com/just-ai/nimbus-cloud-segmentation-using-deep-learning-for-agriculture-5f1320b5c8aa)

Input -> Bootstraping samples -> training -> Post processing -> Output

In the post processing step, the author utilized:
  1. local boundary effect
  2. test time augumentation
  3. Gaussian smoothing
  
which derived from [Kaggle competition](http://blog.kaggle.com/2017/05/09/dstl-satellite-imagery-competition-3rd-place-winners-interview-vladimir-sergey/) (3rd place) 

# Deep Learning in general

[What Do We Understand About Convolutional Networks?](https://arxiv.org/pdf/1803.08834.pdf)

94 pages overview of Convolutional Nerual Network: from technologies to research scope.

# Deep learning in SPPs

__Sadeghi, M., A.A. Asanjan, M. Faridzad, P. Nguyen, K. Hsu, S. Sorooshian, and D. Braithwaite, 2019: PERSIANN-CNN: Precipitation Estimation from Remotely Sensed Information Using Artificial Neural Networks–Convolutional Neural Networks. J. Hydrometeor., 20, 2273–2289, https://doi.org/10.1175/JHM-D-19-0110.1__

Author used CNN to train GOES satellite to map the precipitation from IR band and water vapor channel.
