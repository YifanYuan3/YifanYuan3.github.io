---
title: "Unlocking the Power of Inline Floating-Point Operations on Programmable Switches"
collection: publications
permalink: /publication/fpisa
excerpt: 'This paper proposes a versatile and flexible approach for floating-point number representation, storage, and operations in modern RMT-based programmable switches, which can benefit a wide range of distributed applications, including distributed training and database query. [paper](https://www.usenix.org/conference/nsdi22/presentation/yuan) [arXiv (extended) version](https://arxiv.org/abs/2112.06095) [slides](https://YifanYuan3.github.io/files/fpisa.pptx)'
date: '2022.4.4'
venue: 'NSDI'

---
The advent of switches with programmable dataplanes has enabled the rapid development of new network functionality, as well as providing a platform for acceleration of a broad range of application-level functionality. However, existing switch hardware was not designed with application acceleration in mind, and thus applications requiring operations or datatypes not used in traditional network protocols must resort to expensive workarounds. Applications involving floating point data, including distributed training for machine learning and distributed query processing, are key examples.

In this paper, we propose FPISA, a floating point representation designed to work efficiently in programmable switches. We first implement FPISA on an Intel Tofino switch, but find that it has limitations that impact throughput and accuracy. We then propose hardware changes to address these limitations based on the open-source Banzai switch architecture, and synthesize them in a 15-nm standard-cell library to demonstrate their feasibility. Finally, we use FPISA to implement accelerators for training for machine learning and for query processing, and evaluate their performance on a switch implementing our changes using emulation. We find that FPISA allows distributed training to use 25-75% fewer CPU cores and provide up to 85.9% better throughput in a CPU-constrained environment than SwitchML. For distributed query processing with floating point data, FPISA enables up to 2.7× better throughput than Spark.

[paper](https://www.usenix.org/conference/nsdi22/presentation/yuan) 
[arXiv (extended) version](https://arxiv.org/abs/2112.06095) 
[slides](https://YifanYuan3.github.io/files/fpisa.pptx)