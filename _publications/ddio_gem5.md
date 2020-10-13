---
title: "Data Direct I/O Characterization for Future I/O System Exploration"
collection: publications
permalink: /publication/ddio_gem5
excerpt: 'This paper provides a performance impact of Intel Data Direct I/O technology (DDIO) on applications, and models DDIO in gem5 simulator. [paper](https://YifanYuan3.github.io/files/ddio_ispass2020.pdf)'
date: '2020.8.23'
venue: 'ISPASS'
---
I/O performance plays a critical role in the overall performance of modern servers. The emergence of ultra high-speed I/O devices make the data movement between processor, main memory and devices a major performance bottleneck. Conventionally, the main memory is used as an intermediate buffer between the processor and I/O devices and I/O devices cannot directly access processor side caches. Data Direct I/O (DDIO) technology aims to reduce the memory bandwidth utilization by enabling the I/O devices to leverage Last Level Cache (LLC) as the intermediate buffer. Our experimental results shows that DDIO can completely remove the memory bandwidth utilization while running network or storage intensive applications. However, when modeling I/O subsystem using architectural simulators, DDIO is often ignored, which can result in inaccurate assessments about the I/O and memory subsystem of emerging and future large-scale computer systems. In this paper, we provide a detailed background on DDIO technology in Intel server processors. Then we present our cycle-accurate I/O subsystem model in gem5 simulator that can be configured to model DDIO. We verify our model against baseline gem5 and validate it by comparing its results against a physical computer system.

[paper](https://YifanYuan3.github.io/files/ddio_ispass2020.pdf) 