---
layout: contents
---
# Cache Hierarchy


### A. Overview of Cache Hierarchy with Multiple Levels (L1, L2, L3)

Cache hierarchy consists of multiple levels of cache, typically referred to as L1, L2, and L3 caches. Each level of the cache hierarchy has different capacities, speeds, and proximity to the CPU. 

<br/>

- **L1 Cache**: The closest cache to the CPU, consisting of separate instruction and data caches. It has the smallest capacity but the lowest latency. It stores frequently accessed data and instructions. <br/>

- **L2 Cache**: The secondary cache that is larger in capacity but has higher latency compared to the L1 cache. It acts as a mediator between the L1 cache and the main memory, storing additional data and instructions to reduce the frequency of accessing the main memory. <br/>

- **L3 Cache**: The highest level in the cache hierarchy, typically shared among multiple cores or processors in a multi-core system. It has a larger capacity compared to the L1 and L2 caches, while having a generally higher latency than L1 and L2. The L3 cache provides a larger cache capacity and a shared resource for multiple cores, improving their access to frequently used data and reducing cache conflicts. 

<br/> <br/>

### B. Trade-offs between Cache Size, speed, and Proximity to CPU

Cache hierarchy involves trade-offs between cache size, speed, and proximity to the CPU.

Larger cache sizes can accommodate more data, increasing the chances of cache hits and reducing cache misses. However, larger caches also require more transistors and leads to higher costs. Designers need to balance between cache size, cost, and the expected benefits in terms of improved performance. Different cache organizations, such as direct-mapped, fully associative, or set-associative, have different trade-offs between capacity and access time.

<br/>

- **Direct-mapped Cache**: Each memory block maps to a specific cache location, resulting in simple hardware but potential conflicts.

<br/>

- **Fully Associative Cache**: Any memory block can be stored in any cache location, reducing conflicts but increasing hardware complexity and access time.

<br/>

- **Set Associative Cache**: The cache is divided into multiple sets, allowing each memory block to be mapped to any location within its set. It strikes a balance between direct-mapped and fully associative caches, reducing conflicts while maintaining lower access time compared to fully associative caches.

For caches located closer to the CPU, such as the L1 cache, have lower latency and faster access times. As caches move further away from the CPU, such as the L2 and L3 caches, the latency increases. This trade-off between speed and proximity is influenced by factors like cache organization, technology, and chip layout.

<a href="https://www.researchgate.net/figure/A-classical-three-level-cache-hierarchy_fig1_362707415"><img src="./media/P1.png" alt="Image" height=300>

<br/> <br/>

### C. Retrieval process in Cache Hierarchy

<a href="https://www.researchgate.net/figure/Cache-hit-rate-versus-cache-size-of-the-BS_fig4_353908720"><img src="./media/P3.png" alt="Image" height=300>

If data is not found in the L1 cache (cache miss), the CPU proceeds to check the L2 cache, which is larger but slower than the L1 cache. If the data is present in the L2 cache (cache hit), it is fetched and provided to the CPU, reducing the need to access the main memory.

If data is not found in the L2 cache (cache miss), the CPU then checks the L3 cache or the main memory. The L3 cache, if available, acts as a larger shared cache for multiple cores. If the data is found in the L3 cache (cache hit), it is retrieved and forwarded to the CPU.

When the data is not present in any level of the cache hierarchy (cache miss), it must be fetched from the main memory, leading to a cache miss penalty. The cache hierarchy is designed to minimize memory access time by storing frequently accessed data closer to the CPU, reducing the need for accessing the slower main memory and improving overall system performance.

<a href="(https://www.edn.com/optimizing-for-cache-performance-part-1/)"><img src="./media/P4.png" alt="Image" height=300>

The cache hierarchy is designed in this way to exploit the principle of locality, which states that programs tend to access data and instructions that are spatially or temporally close to each other. By storing frequently accessed data in the smaller and faster cache levels, the CPU can significantly reduce the time required to access data and improve overall system performance.

<a href="https://www.alibabacloud.com/blog/the-mechanism-behind-measuring-cache-access-latency_599384"><img src="./media/P5.png" alt="Image" height=300>

<br/> <br/> <br/>
##### By Lo Wing Sze (55678893)
<br/> <br/>

| [Back to Table of Contents](../table_of_contents.md) | [Back to Home Page](../index.md) |


