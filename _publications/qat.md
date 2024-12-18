---
title: "Intel Accelerators Ecosystem: An SoC-Oriented Perspective"
collection: publications
permalink: /publication/qat
excerpt: 'This is the authentic retrospect of Intel journey of building SoC-level features and software ecosystem for accelerators, and integrating various data accelerators into the modern Xeon CPU chips. [paper](https://ieeexplore.ieee.org/document/10609705)  [slides](https://YifanYuan3.github.io/files/isca2024industry.pptx)'
date: '2024.6.29'
venue: 'ISCA (Industry Track)'

---

A growing demand for hyperscale services has compelled hyperscalers to deploy more compute resources at an unprecedented pace, further accelerated by the demise of Dennard scaling. Meanwhile, a considerable portion of the compute resources are consumed to execute common functions present across the hyperscale services, i.e., datacenter taxes. These challenges motivated many to explore specialized accelerators for these functions. Leading such a technology trend, Intel has integrated diverse on-chip accelerators into its recent flagship datacenter CPU products. Furthermore, to support the easy and efficient use of these accelerators for successful deployment in production hyperscale services, Intel has developed a hardware/software ecosystem.

In this paper, we first focus on Intel’s holistic efforts to build the hardware/software ecosystem, presenting key SoC-level features that facilitate efficient CPU-accelerator interaction, effortless programming and use, and scalable accelerator sharing and virtualization. Next, we delve into the functions, microarchitectures, and software stacks of three new on-chip accelerators: Data Streaming Accelerator (DSA), In-memory Analytics Accelerator (IAA), and Dynamic Load Balancer (DLB). Lastly, we demonstrate that the Intel’s on-chip accelerators can not only significantly reduce the datacenter taxes but also accelerate data-intensive applications essential for hyperscale services, with little effort to use the accelerators.

[paper](https://ieeexplore.ieee.org/document/10609705)

[slides](https://YifanYuan3.github.io/files/isca2024industry.pptx)
