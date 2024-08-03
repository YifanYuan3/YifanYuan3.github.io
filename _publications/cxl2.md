---
title: "Demystifying a CXL Type2 Device: A Heterogeneous Cooperative Computing Perspective"
collection: publications
permalink: /publication/cxl2
excerpt: 'This paper is the first-ever characterization study of real commodity CXL Type-2 devices. We also introduce a real-world use case of Type-2 device as cache-coherent accelerator for Linux kernel function offloading. [paper]() [slides]()'
date: '2024.11.2'
venue: 'MICRO'

---

CXL is the latest interconnect technology built on PCIe, providing three protocols to facilitate three distinct types of devices, each with unique capabilities. Among these devices, a CXL Type-2 device has become commercially available, followed by CXL Type-3 devices. Therefore, it is timely to understand capabilities and characteristics of the CXL Type-2 device, as well as explore suitable applications. In this work, first, we delve into three key features of a CXL Type-2 device: cache-coherent (1) device-accelerator to host-memory, (2) device-accelerator to device-memory, and (3) host-CPU to device-memory accesses. Second, using micro-benchmarks, we comprehensively characterize the latency and bandwidth of these memory accesses with a CXL Type-2 device, and then compare them with those of equivalent memory accesses with comparable devices, such as emulated CXL Type-2, CXL Type-3, and PCIe devices. Lastly, exploiting unique capabilities of a CXL Type-2 device, we propose two CXL-based Linux memory optimization features: compressed RAM cache for swap (zswap) and memory deduplication (ksm), as applications and macro-benchmarks. Our evaluation shows that Redis, when running with traditional CPU-based zswap and ksm, experiences a 4.5–10.3× tail latency increase, compared to Redis running alone. While PCIe-based zswap and ksm still experience a tail latency increase of up to 8.1×, CXL-based zswap and ksm practically eliminate the tail latency increase with faster and more efficient host-device communications than PCIe-based zswap and ksm.


[paper]()

[slides]()