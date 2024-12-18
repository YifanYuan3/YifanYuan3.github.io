---
title: "HALO: Accelerating Flow Classification for Scalable Packet Processing in NFV"
collection: publications
permalink: /publication/halo
excerpt: 'This paper provides a on-CPU near-cache acceleration solution for cuckoo hash lookup, the core operation of modern virtual switch. [paper](https://doi.org/10.1145/3307650.3322272) [slides](https://YifanYuan3.github.io/files/halo.pptx)'
date: '2019.6.22'
venue: 'ISCA'
---
Network Function Virtualization (NFV) has become the new standard in the cloud platform, as it provides the flexibility and agility for deploying various network services on general-purpose servers. 
However, it still suffers from sub-optimal performance in software packet processing. 
Our characterization study of virtual switches shows that the flow classification is the major bottleneck that limits the throughput of the packet processing in NFV, even though a large portion of the classification rules can be cached in the last level cache (LLC) in modern servers. 

To overcome this bottleneck, we propose Halo, an effective near-cache computing solution for accelerating the flow classification. 
Halo exploits the hardware parallelism of the cache architecture consists of Non-Uniform Cache Access (NUCA) and Caching andHome Agent (CHA) available in almost all Intel  multi-core CPUs. 
It associates the accelerator with each CHA component to speed up and scale the flow classification within LLC. 
To make Halo more generic, we extend the x86-64 instruction set with three simple data lookup instructions for utilizing the proposed near-cache accelerators. 
We develop Halo with the full-system simulator gem5. 
The experiments with a variety of real-world workloads of network services demonstrate that Halo improves the throughput of basic flow-rule lookup operations by 3.3×, and scales the representative flow classification algorithm – tuple space search by up to 23.4× with negligible negative impact on the performance of collocated network services, compared with state-of-the-art software-based solutions. 
Halo also performs up to 48.2× more energy-efficient than the fastest but expensive ternary content-addressable memory (TCAM), with trivial power and area overhead.

[paper](https://doi.org/10.1145/3307650.3322272)

[slides](https://YifanYuan3.github.io/files/halo.pptx)