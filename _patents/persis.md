---
title: "Data Consistency and Durability over Distributed Persistent Memory Systems"
collection: patents
permalink: /patent/persis
excerpt : ''
date: 2020.8.5
patent-number: 'US Patent App. 62/986,094'
status: 'pending'
---
Examples described herein relates to a network interface apparatus that includes packet processing circuitry and a bus interface. In some examples, the packet processing circuitry to: process a received packet that includes data, a request to perform a write operation to write the data to a cache, and an indicator that the data is to be durable and based at least on the received packet including the request and the indicator, cause the data to be written to the cache and non-volatile memory. In some examples, the packet processing circuitry is to issue a command to an input output (IO) controller to cause the IO controller to write the data to the cache and the non-volatile memory. In some examples, the cache comprises one or more of: a level-0 (L0), level-1 (L1), level-2 (L2), or last level cache (LLC) and the non-volatile memory comprises one or more of: volatile memory that is part of an Asynchronous DRAM Refresh (ADR) domain, persistent memory, battery-backed memory, or memory device whose state is determinate even if power is interrupted to the memory device. In some examples, based on receipt of a second received packet that includes a request to persist data, the packet processing circuitry is to request that data stored in a memory buffer be copied to the non-volatile memory.


