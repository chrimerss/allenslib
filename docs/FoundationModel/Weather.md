---
layout: default
title: Weather/Climate Foundation Models
parent: Foundation Model in Earth Science
nav_order: 1
---

__[Can AI weather models predict out-of-distribution gray swan tropical cyclones?](https://arxiv.org/pdf/2410.14932)__

This paper investigates how AI weather models predict extreme events such as tropical cyclones and hurricanes. The authors use the NVIDIA ForecastNet model with three experiments: 1. training w/ all cat 3-5 events; 2. partially w/o cat 3-5 events (North Atlantic Ocean or Pacific Ocean); 3. w/o cat 3-5 events.

It is found that AI model cannot extrapolate rare cat 3-5 hurricanes if not trained on them. But if partially trained, say in North Atlantic Ocean, it can be transferred to predict cat 3-5 hurricanes in Pacific Ocean.
