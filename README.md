# learn-socket

1. Basic, non-concurrent examples
   - TTCP: class TCP performance testing tool
   - Round-trip: measure clock error between two hosts.
   - Netcat: a Swiss knife.
   - Slow sink / source.

2. Concurrent examples
   - SOCKS proxy server
     - Relay two TCP connections.
   - Sudoku solver
     - A lot services fit in this request-response model
   - Simple memcached
   - Broadcasting to multiple TCP peers
     - How to deal with slow receiver?

3. Data processing with multiple macines.
   - Parallel N-queues
   - Median of numbers across machines
   - Frequent queries
   - Distributed sorting

4. Advanced topics
   - RPC
     A basic building block for various servers.
   - Load balancings
     Better than round-robin
   - Capacity of a serving system
     - How many machines do I need to support X QPS?
     - What will be the number of replicas of each component? 
   - Fight for (tail) latency
     - Mean and Percentiles: 95%, 99%


## 基础

### 需要关注的性能指标

- Bandwidth(MB/s)
- Throughput
  messages/s, queries/s(QPS),transactions/s(TPS)
- Latency
  milliseconds, percentiles(50% 90% 99% 99.9%)
- Utilization
  percent, payload vs. carrier, goodput vs. theory BW
- Overhead
  CPU usages, for compression and/or encryption

