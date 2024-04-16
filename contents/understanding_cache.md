---
layout: default
---

# Understanding Caches

### A. Comparison of Main memory and Caches
The major difference between caches’ and main meremory’s performance is access speed. As the primary storage unit, main memory is typically built using dynamic random access memory (DRAM), which requires continual refreshing*. Main memory provides a large storage capacity at low cost. Modern main memory is usually built in gigabytes (GB). Generally, main memory is located outside the processor.

On the other hand, caches are built using static random access memory (SRAM), which does not require refreshing*. Caches have a smaller capacity with a higher cost, compared with main memory. It is usually built in megabytes (MB). It is closer to the CPU, and can be placed inside or outside the processor.

With a smaller capacity, caches can only hold a small amount of data. It enables faster search of required data and reduces latency. Meanwhile, the closer proximity of caches allows a shorter data transfer time, which reduces latency and increases access speed.With the aid of the faster SRAM technology, caches can provide 10-100 times faster access to the stored data than the main memory.

| | **Main Memory** | **Cache** |
|:-------------|:------------------|:------|
| **Memory type** | DRAM | SRAM  |
| **Capacity** | Larger | Smaller  |
| **Access Time**| Slower (60–100 nanoseconds) | Faster (1–20 nanoseconds) |

### B. Role of Caches in Reducing Memory Access Time
The cache is crucial in complementing the main memory. The features of fast access time and small capacity make cache suitable for storing frequently accessed data. The CPU can store and retrieve those data more quickly from the cache, reducing the performance bottlenecks in the computer system. As a result, the CPU can operate in a more efficient way and improve system performance.
```
CPU ←→ Cache ←→ Main memory
```

##### By Cheng Man Ho (56612619)
[Back to Table of Contents](./table_of_contents.md)
