---
title: "Nomad: Non-Exclusive Memory Tiering via Transactional Page Migration"
collection: publications
permalink: /publication/nomad
excerpt: 'This paper presents a novel tiered memory management software system based on emerging CXL memory. '
date: '2024.7.10'
venue: 'OSDI'

---

With the advent of byte-addressable memory devices, such as CXL memory, persistent memory, and storage-class memory, tiered memory systems have become a reality. Page migration is the de facto method within operating systems for managing tiered memory. It aims to bring hot data whenever possible into fast memory to optimize the performance of data accesses while using slow memory to accommodate data spilled from fast memory. While the existing research has demonstrated the effectiveness of various optimizations on page migration, it falls short of addressing a fundamental question: Is exclusive memory tiering, in which a page is either present in fast memory or slow memory, but not both simultaneously, the optimal strategy for tiered memory management?


We demonstrate that page migration-based exclusive memory tiering suffers significant performance degradation when fast memory is under pressure. In this paper, we propose non- exclusive memory tiering, a page management strategy that retains a copy of pages recently promoted from slow memory to fast memory to mitigate memory thrashing. To enable non-exclusive memory tiering, we develop NOMAD, a new page management mechanism for Linux that features transactional page migration and page shadowing. NOMAD helps remove page migration off the critical path of program execution and makes migration completely asynchronous. Evaluations with carefully crafted micro-benchmarks and real-world applications show that NOMAD is able to achieve up to 6x performance improvement over the state-of-the-art transparent page placement (TPP) approach in Linux when under memory pressure. We also compare NOMAD with a recently proposed access sampling-based page migration approach and demonstrate NOMAD’s strengths and potential weaknesses in various scenarios. Through the evaluation of NOMAD, we discover a serious issue facing all tested approaches, unfortunately including NOMAD, and call for further research on tiered memory-aware memory allocation.
