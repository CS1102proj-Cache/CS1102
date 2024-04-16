---
layout: default
---

# Principles of Cache Operation

### A. Locality: Temporal and spatial locality

Caches’ operation is based on the principle of locality of reference, which describes that programs tend to access the same set of data or the data with nearby addresses. There are two types of locality, temporal and spatial. Temporal locality refers to the tendency of accessing the same data again in the near future, while spatial locality refers to the tendency of accessing  the data with addresses near to the current data in the near future. Locality is common in loop instructions as some variables are accessed again and again. For example, in the following loop,

```js
sum = 0;
for (i = 0; i < 5; i++) {
	sum += a[i];
}
return sum;
```

the variable _sum_ is accessed repeatedly during every iteration, illustrating the presence of temporal locality. On the other hand, the array elements a[i] are accessed in consecutive order, demonstrating spatial locality.
Taking advantage of the principle, these two types of data are stored in the cache, to increase the likelihood that the CPU can have faster access to the required data. 

### B. Performance Evaluation: Cache Hits and Cache Misses

If the cache contains the required data, there will be a cache hit, which is defined as a successful data retrieval from cache. In contrast, an unsuccessful data retrieval from cache is called a cache miss*. A cache miss results in a cache miss penalty, which is the additional time or delay incurred. If the required data are not stored in cache, they will be fetched from a slower memory unit like main memory. Consequently, the memory access time would increase.
Cache performance can be measured by hit rate and miss rate. Hit rate is the percentage of cache hits,

|_Hit rate_ =  (Number of cache hits / Number of cache accesses) * 100%|
|:-------------|

On the other hand, miss rate is the percentage of cache misses,

|_Miss rate_ =  (Number of cache misses / Number of cache accesses) * 100%  <span style="color: red;">OR</span>  1 - hit rate|
|:-------------|

- Ideal hit rate >= 95%
- Ideal miss rate <= 5% 

Average memory access time can be calculated using the following formula:
**Average memory access time** = Number of Cache hits + Miss rate * Cache Miss penalty

[* More information about different types of cache misses](https://www.hostinger.com/tutorials/cache-miss#What_Is_a_Cache_Miss)

##### By Cheng Man Ho (56612619)
  
[Back to Table of Contents](../table_of_contents.md) |
[Back to Home Page](../index.md)
