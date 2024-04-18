---
layout: contents
title: Understanding Caches
---

#### Understanding Caches

##### A. Comparison of Main Memory and Caches
The major difference between caches’ and main memory’s performance is access speed. As the primary storage unit, main memory is typically built using dynamic random access memory (DRAM), which requires continual refreshing*. Main memory provides a large storage capacity at a low cost. Modern main memory is usually built-in gigabytes (GB). Generally, the main memory is located outside the processor.

On the other hand, caches are built using static random access memory (SRAM), which does not require refreshing*. Caches have a smaller capacity with a higher cost, compared with main memory. It is usually built in megabytes (MB). It is closer to the CPU, and can be placed inside or outside the processor.

With a smaller capacity, caches can only hold a small amount of data. It enables faster search of required data and reduces latency. Meanwhile, the closer proximity of caches allows a shorter data transfer time, which reduces latency and increases access speed. With the aid of the faster SRAM technology, caches can provide 10-100 times faster access to the stored data than the main memory.

| | **Main Memory** | **Cache** |
|:-------------|:------------------|:------|
| **Memory type** | DRAM | SRAM  |
| **Capacity** | Larger | Smaller  |
| **Access Time**| Slower (60–100 nanoseconds) | Faster (1–20 nanoseconds) |
  
[* More information about DRAM and SRAM](https://www.diffen.com/difference/Dynamic_random-access_memory_vs_Static_random-access_memory)


<br/> <br/> <br/>
###### By Cheng Man Ho (56612619)
<br/> <br/>

[Previous: Introduction](./introduction.md) | [Next: Principles of Cache Operation](./principles_of_cache_operation.md) <br/>
[Back to Table of Contents](../table_of_contents.md) | [Back to Home Page](../index.md)
