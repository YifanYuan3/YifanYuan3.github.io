---
title: "QEI: Query Acceleration Can be Generic and Efficient in the Cloud"
collection: publications
permalink: /publication/qei
excerpt: 'This paper proposes a generic accelerator architecture for fine-gained latency-sensitive queries in various data structures. It also proposes a hybrid scheme for the accelerator to be efficiently integrated into modern server CPU. [paper](https://ieeexplore.ieee.org/document/9407097) [slides](https://YifanYuan3.github.io/files/qei.pptx)'
date: '2021.2.27'
venue: 'HPCA'
---
Data query operations of different data structures are ubiquitous and critical in today's data center infrastructures and applications. 
However, query operations are not always performance-optimal to be executed on general-purpose CPU cores. 
These operations exhibit insufficient memory-level parallelism and frontend bottlenecks due to unstructured control flow. 
Furthermore, the data access patterns are not cache- or prefetch-friendly.
Based on our performance analysis on a commodity server, query operations can consume a large percentage of the CPU cycles in various modern cloud workloads. 
Existing accelerator solutions for query operations do not strike a balance between their generality, scalability, latency, and hardware complexity. 

In this paper, we propose QEI, a generic, integrated, and efficient acceleration solution for various data structure queries. 
We first abstract the query operations to a few regular steps and map them to a simple and hardware-friendly configurable finite automaton model. 
Based on this model, we develop the QEI architecture that allows multiple query operations to execute in parallel to maximize throughput. 
We also propose a novel way to integrate the accelerator into the CPU that balances performance, latency, and hardware cost.
QEI keeps the main control logic near the L2 cache to leverage existing hardware resources in the core while distributing the data-intensive comparison logic to each last-level cache slice for higher parallelism.
Our results with five representative data center workloads show that QEI can achieve 6.5x~11.2x performance improvement in various scenarios with low overhead. 

[paper](https://ieeexplore.ieee.org/document/9407097) [slides](https://YifanYuan3.github.io/files/qei.pptx)