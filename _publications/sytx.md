---
title: "STYX: Exploiting SmartNIC Capability to Reduce Datacenter Memory Tax"
collection: publications
permalink: /publication/styx
excerpt: 'This paper proposes to take advantage of the capability of SmartNICs in the datacenter to offload a set of expensive kernel memory management tasks, so that the CPU cycles and cache pollution can be significantly reduced. [paper (including video and slides)](https://www.usenix.org/conference/atc23/presentation/ji) '
date: '2023.7.10'
venue: 'ATC'

---

Memory optimization kernel features, such as memory deduplication, are designed to improve the overall efficiency of systems like datacenter servers, and they have proven to be effective. However, when invoked, these kernel features notably disrupt the execution of applications, intensively consuming the server CPU's cycles and polluting its caches. To minimize such disruption, we propose STYX, a framework for offloading the intensive operations of these kernel features to SmartNIC (SNIC). STYX first RDMA-copies the server's memory regions, on which these kernel features intend to operate, to an SNIC's memory region, exploiting SNIC's RDMA capability. Subsequently, leveraging SNIC's (underutilized) compute capability, STYX makes the SNIC CPU perform the intensive operations of these kernel features. Lastly, STYX RDMA-copies their results back to a server's memory region, based on which it performs the remaining operations of the kernel features. To demonstrate the efficacy of STYX, we re-implement two memory optimization kernel features in Linux: (1) memory deduplication (ksm) and (2) compressed cache for swap pages (zswap), using the STYX framework. We then show that a system with STYX provides a 55-89% decrease in 99th-percentile latency of co-running applications, compared to a system without STYX, while preserving the benefits of these kernel features.


[paper (including video and slides)](https://www.usenix.org/conference/atc23/presentation/ji)
