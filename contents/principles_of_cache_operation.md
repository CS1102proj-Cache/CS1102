---
layout: contents
title: Principles of Cache Operation
---
<body>
<h4><b>Principles of Cache Operation</b></h4>

<h5><b>A. Locality: Temporal and spatial locality</b></h5>

<div class="bodytext">
Caches’ operation is based on the principle of locality of reference, which describes that programs tend to access the same set of data or the data with nearby addresses. There are two types of locality, temporal and spatial. <br/>

<li><b>Temporal locality</b>: the tendency of accessing the same data again shortly </li>
<li><b>Spatial locality</b>: the tendency of accessing the data with addresses near the current data shortly</li>
<br/>
Locality is common in loop instructions as some variables are accessed again and again. For example, in the following loop, <br/>

<pre>
<code>
sum = 0;
for (i = 0; i < 5; i++) {
	sum += a[i];
}
return sum;
</code>
</pre>

<br/>
the variable <i>sum</i> is accessed repeatedly during every iteration, illustrating the presence of temporal locality. On the other hand, the array elements a[i] are accessed in consecutive order, demonstrating spatial locality.
Taking advantage of the principle, these two types of data are stored in the cache, to increase the likelihood that the CPU can have faster access to the required data. 

<br/> <br/>

<h5><b>B. Performance Evaluation: Cache Hits and Cache Misses</b></h5>

If the cache contains the required data, there will be a cache hit, which is defined as a successful data retrieval from the cache. In contrast, an unsuccessful data retrieval from the cache is called a cache miss*. A cache miss results in a cache miss penalty, which is the additional time or delay incurred. If the required data are not stored in the cache, they will be fetched from a slower memory unit like main memory. Consequently, the memory access time would increase.
Cache performance can be measured by hit rate and miss rate. Hit rate is the percentage of cache hits, <br/> <br/>

<b><i>Hit rate</i></b> =  (Number of cache hits / Number of cache accesses) * 100% <br/><br/>

On the other hand, miss rate is the percentage of cache misses, <br/><br/>

<b><i>Miss rate</i></b> =  (Number of cache misses / Number of cache accesses) * 100%  <span style="color: red;">OR</span>  1 - hit rate <br/><br/>

<li>Ideal hit rate >= 95%</li>
<li>Ideal miss rate <= 5%</li>
<br/>
Average memory access time can be calculated using the following formula: <br/>
<b>Average memory access time</b> = Number of Cache hits + Miss rate * Cache Miss penalty

<br/><br/>

<a href="https://www.hostinger.com/tutorials/cache-miss#What_Is_a_Cache_Miss">* More information about different types of cache misses</a>

<br/> <br/> <br/>
<h6>By Cheng Man Ho (56612619)</h6>
<br/> <br/>
<div class="middle"><b>
<a href="https://cs1102proj-cache.github.io/CS1102/contents/understanding_cache.html">Previous: Understanding Cache</a> |
<a href="https://cs1102proj-cache.github.io/CS1102/contents/cache_hierarchy.html">Next: Cache Hierarchy</a></b>
<br/> 
