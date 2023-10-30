---
title: "Demystifying CXL Memory with Genuine CXL-Ready Systems and Devices"
collection: publications
permalink: /publication/memo
excerpt: 'This paper is the first-ever characterization study of real commodity CXL memory devices. We develop and open-source MEMO benchmark for CXL memory testing, and develop a auto-tuning algorithm to make the most out of the CXL devices as not only capacity expander but also bandwidth expander. [arXiv version](https://arxiv.org/abs/2303.15375) [slides](https://YifanYuan3.github.io/files/cxl-micro23.pptx)'
date: '2023.10.28'
venue: 'MICRO'

---

The ever-growing demands of memory capacity and bandwidth by datacenter servers has driven recent innovations on memory expansion and disaggregation technologies based on Compute eXpress Link (CXL). Especially, the CXL-based memory expansion technology has gained notable attention recently for its ability of not only economically expanding memory capacity and bandwidth, but also decoupling memory technologies from specific memory interfaces of the CPU. However, CXL memory devices and systems supporting them have not been widely available. Recent studies on performance characterizations and efficient uses of CXL memory commonly treat CXL-memory systems as conventional NUMA systems---CXL memory is emulated as a remote NUMA node in a multi-socket system.

In this paper, we first evaluate true CXL-ready systems based on the latest 4th-generation Intel Xeon CPU with three CXL memory devices from different manufacturers. Specifically, we run a set of microbenchmarks not only to compare the performance of true CXL memory with that of emulated CXL memory (i.e., DDR memory in a remote NUMA node), but also to analyze the complex interplay between the CPU and CXL memory in depth. This divulges important differences between emulated and true CXL memory devices, some of which will compel researchers to revisit analyses and proposals of recent work. Second, we identify opportunities for memory-intensive applications to benefit from using CXL memory. Lastly, based on these observations, we propose a CXL-memory-aware dynamic page allocation policy, Caption to use CXL memory more efficiently. We show that Caption can automatically converge to an empirically favorable page allocation ratio and improve performance of memory-intensive applications by up to 81%, compare to the default page allocation policy designed for traditional NUMA systems.


[arXiv version](https://arxiv.org/abs/2303.15375)

[slides](https://YifanYuan3.github.io/files/cxl-micro23.pptx)