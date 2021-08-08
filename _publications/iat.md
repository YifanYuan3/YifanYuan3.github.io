---
title: "Don't Forget the I/O When Allocating Your LLC"
collection: publications
permalink: /publication/iat
excerpt: 'This paper proposes the first I/O-aware LLC management mechanism for performance isolation in DDIO-enable platform. [paper](https://ieeexplore.ieee.org/document/9499850) [arXiv version](https://arxiv.org/abs/2007.04552) [slides](https://YifanYuan3.github.io/files/iat.pptx)'
date: '2021.6.14'
venue: 'ISCA'
---
In modern server CPUs, last-level cache (LLC) is a critical hardware resource that exerts significant influence on the performance of the workloads, and how to manage LLC is a key to the performance isolation and QoS in the cloud with multi-tenancy. In this paper, we argue that in addition to CPU cores, high-speed I/O is also important for LLC management. This is because of an Intel architectural innovation -- Data Direct I/O (DDIO) -- that directly injects the inbound I/O traffic to (part of) the LLC instead of the main memory. We summarize two problems caused by DDIO and show that (1) the default DDIO configuration may not always achieve optimal performance, (2) DDIO can decrease the performance of non-I/O workloads that share LLC with it by as high as 32%.

We then present IAT, the first LLC management mechanism that treats the I/O as the first-class citizen. IAT monitors and analyzes the performance of the core/LLC/DDIO using CPU's hardware performance counters and adaptively adjusts the number of LLC ways for DDIO or the tenants that demand more LLC capacity. In addition, IAT dynamically chooses the tenants that share its LLC resource with DDIO to minimize the performance interference by both the tenants and the I/O. Our experiments with multiple microbenchmarks and real-world applications demonstrate that with minimal overhead, IAT can effectively and stably reduce the performance degradation caused by DDIO.

[paper](https://ieeexplore.ieee.org/document/9499850)
[arXiv version](https://arxiv.org/abs/2007.04552)
[slides](https://YifanYuan3.github.io/files/iat.pptx)