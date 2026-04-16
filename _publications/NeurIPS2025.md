---
title: "Proxy Target: Bridging the Gap Between Discrete Spiking Neural Networks and Continuous Control"
collection: publications
category: conferences
permalink: /publication/NeurIPS2025
excerpt: 'Standard continuous-control RL methods are incompatible with SNN dynamics, causing unstable training and poor performance. This paper introduces a proxy target network that stabilizes learning and boosts performance without affecting inference efficiency, enabling SNNs to outperform ANNs in some settings.'
date: 2024-02-17
venue: 'The Thirty-ninth Annual Conference on Neural Information Processing Systems (NeurIPS)'
paperurl: 'https://openreview.net/forum?id=RRBve5GwjS'
citation: 'Zijie XU, Tong Bu, Zecheng Hao, Jianhao Ding, Zhaofei Yu.  Annual Conference on Neural Information Processing Systems (NeurIPS) 2025.'
---

[OpenReview](https://openreview.net/forum?id=RRBve5GwjS) [Arxiv](https://arxiv.org/abs/2505.24161) [Github](https://github.com/xuzijie32/Proxy-Target)


Abstract: Spiking Neural Networks (SNNs) offer low-latency and energy-efficient decision making on neuromorphic hardware, making them attractive for Reinforcement Learning (RL) in resource-constrained edge devices. However, most RL algorithms for continuous control are designed for Artificial Neural Networks (ANNs), particularly the target network soft update mechanism, which conflicts with the discrete and non-differentiable dynamics of spiking neurons. We show that this mismatch destabilizes SNN training and degrades performance. To bridge the gap between discrete SNNs and continuous-control algorithms, we propose a novel proxy target framework. The proxy network introduces continuous and differentiable dynamics that enable smooth target updates, stabilizing the learning process. Since the proxy operates only during training, the deployed SNN remains fully energy-efficient with no additional inference overhead. Extensive experiments on continuous control benchmarks demonstrate that our framework consistently improves stability and achieves up to $32\%$ higher performance across various spiking neuron models. Notably, to the best of our knowledge, this is the first approach that enables SNNs with simple Leaky Integrate and Fire (LIF) neurons to surpass their ANN counterparts in continuous control. This work highlights the importance of SNN-tailored RL algorithms and paves the way for neuromorphic agents that combine high performance with low power consumption. Code is available at https://github.com/xuzijie32/Proxy-Target.
