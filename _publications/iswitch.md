---
title: "Accelerating Distributed Reinforcement Learning with In-Switch Computing"
collection: publications
permalink: /publication/iswitch
excerpt: 'This paper presents an algorithm/hardware co-design to accelerate gradient aggregation in distributed reinforcement learning training. [paper](https://doi.org/10.1145/3307650.3322259)  [slides](https://YifanYuan3.github.io/files/iswitch.pdf)'
date: '2019.6.22'
venue: 'NSDI (poseter), ISCA (full paper)'
---
Reinforcement learning (RL) has attracted much attention recently, as new and emerging AI-based applications are demanding the capabilities to intelligently react to environment changes. Unlike distributed deep neural network (DNN) training, the distributed RL training has its unique workload characteristics - it generates orders of magnitude more iterations with much smaller sized but more frequent gradient aggregations. More specifically, our study with typical RL algorithms shows that their distributed training is latency critical and that the network communication for gradient aggregation occupies up to 83.2% of the execution time of each training iteration.

In this paper, we present iSwitch, an in-switch acceleration solution that moves the gradient aggregation from server nodes into the network switches, thus we can reduce the number of network hops for gradient aggregation. This not only reduces the end-to-end network latency for synchronous training, but also improves the convergence with faster weight updates for asynchronous training. Upon the in-switch accelerator, we further reduce the synchronization overhead by conducting on-the-fly gradient aggregation at the granularity of network packets rather than gradient vectors. Moreover, we rethink the distributed RL training algorithms and also propose a hierarchical aggregation mechanism to further increase the parallelism and scalability of the distributed RL training at rack scale.

We implement iSwitch using a real-world programmable switch NetFPGA board. We extend the control and data plane of the programmable switch to support iSwitch without affecting its regular network functions. Compared with state-of-the-art distributed training approaches, iSwitch offers a system-level speedup of up to 3.66× for synchronous distributed training and 3.71× for asynchronous distributed training, while achieving better scalability.


[paper](https://doi.org/10.1145/3307650.3322259)

[slides](https://YifanYuan3.github.io/files/iswitch.pdf)