---
title: "Efficiently Merging Non-identical Pages in Kernel Same-page Merging (KSM) for Efficient and Im- proved Memory Deduplication and Security"
collection: patents
permalink: /patent/ksmdsa
excerpt : ' '
date: 2023.9.15
patent-number: 'US Patent App. 18/369,080'
status: 'pending'
---
Methods and apparatus for efficiently merging non-identical pages in Kernel Same-page Merging (KSM) for efficient and improved memory deduplication and security. The methods and apparatus identify memory pages with similar data and selectively merge those pages based on criteria such as a threshold. Memory pages in memory for a computing platform are scanned to identify pages storing similar but not identical data. A delta record between the similar memory pages is created, and it is determined whether a size of the delta (i.e., amount of content that is different) is less than a threshold. If so, the delta record is used to merge the pages. In one aspect, operations for creating delta records and merging the content of memory pages using delta records is offloaded from a platform's CPU. Support for memory reads and memory writes are provided utilizing delta records, including merging and unmerging pages under applicable conditions.