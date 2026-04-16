---
title: "CaRe-BN: Precise Moving Statistics for Stabilizing Spiking Neural Networks in Reinforcement Learning"
collection: publications
category: conferences
permalink: /publication/CaRe_BN
excerpt: 'CaRe-BN improves training stability in Spiking Neural Networks for reinforcement learning by adapting and recalibrating batch normalization statistics, leading to faster convergence and better policies. It boosts SNN performance (even surpassing ANNs) without affecting inference efficiency, making it suitable for energy-constrained deployment.'
date: 2026
venue: 'The Fourteenth International Conference on Learning Representations'
paperurl: 'https://openreview.net/forum?id=AaZVrbElhC'
citation: 'Zijie XU, Tong Bu, Zecheng Hao, Jianhao Ding, Zhaofei Yu.  Annual Conference on Neural Information Processing Systems (NeurIPS) 2025.'
---

[OpenReview](https://openreview.net/forum?id=AaZVrbElhC) [Arxiv](https://arxiv.org/abs/2509.23791) [Github](https://github.com/xuzijie32/CaRe-BN)

Abstract: Spiking Neural Networks (SNNs) offer low-latency and energy-efficient decision-making on neuromorphic hardware by mimicking the event-driven dynamics of biological neurons. However, the discrete and non-differentiable nature of spikes leads to unstable gradient propagation in directly trained SNNs, making Batch Normalization (BN) an important component for stabilizing training. In online Reinforcement Learning (RL), imprecise BN statistics hinder exploitation, resulting in slower convergence and suboptimal policies. While Artificial Neural Networks (ANNs) can often omit BN, SNNs critically depend on it, limiting the adoption of SNNs for energy-efficient control on resource-constrained devices. To overcome this, we propose Confidence-adaptive and Re-calibration Batch Normalization (CaRe-BN), which introduces (i) a confidence-guided adaptive update strategy for BN statistics and (ii) a re-calibration mechanism to align distributions. By providing more accurate normalization, CaRe-BN stabilizes SNN optimization without disrupting the RL training process. Importantly, CaRe-BN does not alter inference, thus preserving the energy efficiency of SNNs in deployment. Extensive experiments on both discrete and continuous control benchmarks demonstrate that CaRe-BN improves SNN performance by up to 22.6% across different spiking neuron models and RL algorithms. Remarkably, SNNs equipped with CaRe-BN even surpass their ANN counterparts by 5.9%. These results highlight a new direction for BN techniques tailored to RL, paving the way for neuromorphic agents that are both efficient and high-performing. Code is available at https://github.com/xuzijie32/CaRe-BN.

Bibtex: 
```
@inproceedings{
xu2026carebn,
title={CaRe-{BN}: Precise Moving Statistics for Stabilizing Spiking Neural Networks in Reinforcement Learning},
author={Zijie Xu and Xinyu Shi and Yiting Dong and Zihan Huang and Zhaofei Yu},
booktitle={The Fourteenth International Conference on Learning Representations},
year={2026},
url={https://openreview.net/forum?id=AaZVrbElhC}
}
```
