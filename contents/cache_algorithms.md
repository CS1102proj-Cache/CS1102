---
layout: contents
Title: Cache Algorithms
---

<body>
<h4><b>Cache Algorithms</b></h4>

<h5><b>A. LRU, LFU and Random</b></h5>

LRU, LFU, and random are the common cache replacement policies. <br/>

<a href="https://dev.to/satrobit/cache-replacement-algorithms-how-to-efficiently-manage-the-cache-storage-2ne1"><img src="./media/P2.png" alt="Image" height=300 width=auto></a>  <br/><br/>


<b>LRU (Least Recently Used)</b> <br/>
LRU represents the least recently used algorithm and it is one of the most famous algorithms. The name LRU implies that it keeps the least recently used objects at the top and evicts objects that have not been used when the list reaches the maximum capacity.  <br/>
<ul><li>Benefits </li>
  <ul>
  <li>It is fast and efficient in the view of cache management. The high-efficiency benefits for the applications that need quick access to used data. </li> 
  <li>LRU can work well with data subject to locality concerns, showing that it is effective for applications where recently accessed items are likely to be accessed again soon. This attribute makes it suitable for applications with temporal locality. </li> </ul> </ul><br/>
<ul><li>Drawbacks </li>
  <ul>
  <li>It would perform poorly when element files are accessed occasionally but consistently while other elements are accessed very frequently for a short duration and never accessed again. It would lead to inefficiency of cache utilization. </li> 
  <li>A larger cache size is required to boost the efficiency. </li> </ul></ul><br/> <br/>

<b>LFU (Least Frequently Used)</b> <br/>
LFU means the least frequently used algorithm and it monitors how many times it was accessed. Each object is associated with a counter which counts how many times it was accessed. If the list reaches the maximum capacity, objects with the lowest counters are evicted.  <br/>
<ul><li>Benefits </li>
  <ul>
  <li>Cache pollution can be avoided by evicting items that are accessed once or rarely, regardless of their recency.  </li> 
  <li>It can keep items that are accessed more often than others and can manage cyclic access patterns better than LRU. </li> </ul> </ul><br/>
<ul><li>Drawbacks </li>
  <ul>
  <li>It would be ineffective for applications with evolving access patterns as the items that were popular in the past may not be popular in the present or future. </li> </ul></ul><br/> <br/>

<b>Random</b> <br/>
In a random algorithm, it works very simple. It randomly selects an object and evicts it when it reaches maximum capacity. Every cache entry has the same probability of being replaced. <br/>
<ul><li>Benefits </li>
  <ul>
  <li>It is easy and simple to implement because it does not keep references or the history of the items. </li> </ul> </ul><br/>
<ul><li>Drawbacks </li>
  <ul>
  <li>It would lead to suboptimal cache performance by comparing with other complicated policies. It does not take the usage pattern or the possibility of future access into account. </li> </ul></ul><br/> <br/>

Every algorithm contains its advantages and disadvantages in using it, people should use it depending on the specific needs of the system. <br/> <br/>

<h5><b>B. Impact of cache algorithms on cache hit rates</b></h5>
The cache algorithms are crucial in affecting the cache hit rates. The cache replacement policy determines which object to be evicted if a new object is inserted. The LRU and LFU would enhance the possibility of cache hits as they keep recently accessed data and frequently used data. The random replacement would result in poor hit rates due to the random nature of eviction.

<br/> <br/> <br/>
<h6>By Ng Wing Hei (56612889)</h6>
<br/> <br/>
<a href="https://github.com/CS1102proj-Cache/CS1102/blob/main/contents/cache_algorithms.md?plain=1">Click to view the source code of this page.</a>
<br/> <br/>
<div class="middle">
<a href="https://cs1102proj-cache.github.io/CS1102/contents/cache_hierarchy.html">Previous: Cache Hierarchy</a> |
<a href="https://cs1102proj-cache.github.io/CS1102/contents/acceleration_of_memory_access.html">Next: Acceleration of Memory Access</a>
<br/> 
