---
layout: contents
title: Understanding Caches
---

<body>
<h4><b>Understanding Caches</b></h4>

<h5><b>A. Comparison of Main Memory and Caches</b></h5>
<div class="bodytext">
Access speed is the major difference between caches and main memory.  As the primary storage unit, main memory is typically built using dynamic random access memory (DRAM), which requires continual refreshing*. Main memory provides a large storage capacity at a low cost. ⁤⁤Modern main memory is usually built-in gigabytes (GB). Generally, the main memory is located outside the processor. <br/><br/>

On the other hand, caches are built using static random access memory (SRAM), which does not require refreshing*. Caches have a smaller capacity at a higher cost than main memory. It is usually built in megabytes (MB). It is located closer to the CPU and can be placed inside or outside the processor. <br/><br/>

With a smaller capacity, caches can only hold a small amount of data, but it enables faster data search and reduces latency. Meanwhile, the close proximity of caches allows a shorter data transfer time, which reduces latency and increases access speed. With the aid of faster SRAM technology, caches can provide 10-100 times faster access to the stored data than the main memory.
<br/><br/>
  <table>
    <thead>
      <tr>
        <th></th>
        <th><b>Main Memory</b></th>
        <th><b>Cache</b></th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td><b>Memory type</b></td>
        <td>DRAM</td>
        <td>SRAM</td>
      </tr>
      <tr>
        <td><b>Capacity</b></td>
        <td>Larger</td>
        <td>Smaller</td>
      </tr>
      <tr>
        <td><b>Access Time</b></td>
        <td>Slower (60–100 nanoseconds)</td>
        <td>Faster (1–20 nanoseconds)</td>
      </tr>
    </tbody>
  </table>

<br/> <br/>

<a href="https://www.diffen.com/difference/Dynamic_random-access_memory_vs_Static_random-access_memory">* More information about DRAM and SRAM</a>

<br/> <br/> <br/>
<h6>By Cheng Man Ho (56612619)</h6>
<br/> <br/>
<a href="https://github.com/CS1102proj-Cache/CS1102/blob/main/contents/understanding_cache.md?plain=1">Click to view source code of this page.</a>
<br/> <br/>
<div class="middle">
<a href="https://cs1102proj-cache.github.io/CS1102/contents/introduction.html">Previous: Introduction</a> | 
<a href="https://cs1102proj-cache.github.io/CS1102/contents/principles_of_cache_operation.html">Next: Principles of Cache Operation</a><br/>
