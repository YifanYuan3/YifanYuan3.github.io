---
title: "Offload of Data Lookup Operations"
collection: patents
permalink: /patent/halo
excerpt: 'The corresponding patent of HALO.'
date: 2019.4.4
patent-number: 'US Patent App. 16/207,065'
status: 'pending'
---
A central processing unit can offload table lookup or tree traversal to an offload engine. The offload engine can provide hardware accelerated operations such as instruction queueing, bit masking, hashing functions, data comparisons, a results queue, and a progress tracking. The offload engine can be associated with a last level cache. In the case of a hash table lookup, the offload engine can apply a hashing function to a key to generate a signature, apply a comparator to compare signatures against the generated signature, retrieve a key associated with the signature, and apply the comparator to compare the key against the retrieved key. Accordingly, a data pointer associated with the key can be provided in the result queue. Acceleration of operations in tree traversal and tuple search can also occur.