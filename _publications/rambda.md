---
title: "RAMBDA: RDMA-driven Acceleration Framework for Memory-intensive us-scale Datacenter Applications"
collection: publications
permalink: /publication/rambda
excerpt: 'Responding to the "datacenter tax" and "killer microseconds" problems, this paper proposes a holistic solution for us-scale datacenter applications accelerations, leveraging emerging RDMA and cache-coherent accelerator techniques. [paper](https://ieeexplore.ieee.org/abstract/document/10071127) [arXiv version](https://arxiv.org/abs/2203.08906) [slides](https://YifanYuan3.github.io/files/rambda.pptx)'
date: '2023.2.25'
venue: 'HPCA'

---
Responding to the "datacenter tax" and "killer microseconds" problems for memory-intensive datacenter applications, diverse solutions including Smart NIC-based ones have been proposed. Nonetheless, they often suffer from high overhead of communications over network and/or PCIe links. To tackle the limitations of the current solutions, this paper proposes RAMBDA, a holistic network and architecture co-design solution that leverages current RDMA and emerging cache-coherent off-chip interconnect technologies. Specifically, RAMBDA consists of four hardware and software components: 
(1) unified abstraction of inter- and intra-machine communications synergistically managed by one-sided RDMA write and cache-coherent memory write; 
(2) efficient notification of requests to accelerators assisted by cache coherence; 
(3) cache-coherent accelerator architecture directly interacting with NIC; and  
(4) adaptive device-to-host data transfer for modern server memory systems comprising both DRAM and NVM exploiting state-of-the-art features in CPUs and PCIe.
We prototype RAMBDA with a commercial system and evaluate three popular datacenter applications: (1) in-memory key-value store, (2) chain replication-based distributed transaction system, and (3) deep learning recommendation model inference. The evaluation shows that RAMBDA provides 30.1~69.1% lower latency,  0.2~2.5X throughput, and ~3X higher energy efficiency than the current state-of-the-art solutions, including Smart NIC. For those cases where RAMBDA perform poorly, we also also envision future architecture to improve it.

[paper](https://ieeexplore.ieee.org/abstract/document/10071127) 
[arXiv version](https://arxiv.org/abs/2203.08906) 
[slides](https://YifanYuan3.github.io/files/rambda.pptx)
