---
title: "Intel Accelerators Ecosystem: An SoC-Oriented Perspective"
collection: publications
permalink: /publication/qat
excerpt: 'This is the authentic retrospect of Intel journey of building SoC-level features and software ecosystem for accelerators, and integrating various data accelerators into the modern Xeon CPU chips. [paper](https://ieeexplore.ieee.org/document/10609705)  [slides](https://YifanYuan3.github.io/files/isca2024industry.pptx)'
date: '2024.6.29'
venue: 'ISCA (Industry Track)'

---

As semiconductor power density is no longer constant with the technology process scaling down, modern CPUs are integrating capable data accelerators on chip, aiming to improve performance and efficiency for a wide range of applications and usages. One such accelerator is the Intel Data Streaming Accelerator (DSA) introduced in Intel 4th Generation Xeon Scalable CPUs (Sapphire Rapids). DSA targets data movement operations in memory that are common sources of overhead in datacenter workloads and infrastructure. In addition, it becomes much more versatile by supporting a wider range of operations on streaming data, such as CRC32 calculations, delta record creation/merging, and data integrity field (DIF) operations. This paper sets out to introduce the latest features supported by DSA, deep-dive into its versatility, and analyze its throughput benefits through a comprehensive evaluation. Along with the analysis of its characteristics, and the rich software ecosystem of DSA, we summarize several insights and guidelines for the programmer to make the most out of DSA, and use an in-depth case study of DPDK Vhost to demonstrate how these guidelines benefit a real application.

[paper](https://ieeexplore.ieee.org/document/10609705)

[slides](https://YifanYuan3.github.io/files/isca2024industry.pptx)
