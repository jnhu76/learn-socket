# SOCKET基础

## 性能指标

需要关注的性能指标

- Bandwidth(MB/s)
- Throughput
  messages/s, queries/s(QPS),transactions/s(TPS)
- Latency
  milliseconds, percentiles(50% 90% 99% 99.9%)
- Utilization
  percent, payload vs. carrier, goodput vs. theory BW
- Overhead
  CPU usages, for compression and/or encryption

## SOCKET api

基础api： `socket`, `listen`, `bind`, `accept`, `connect`, `read/recv`, `write/send`, `shutdown`, `close`, etc.

## todo：优化 TTCP

1. Measure throughput(message/s) and latency
2. Server supports concurrent clients.
3. Multiple sessions/connections, test fairness of TCP
4. Lone-fat pipe, cross data centers
   - Pipelining
5. Nagles's algorithm and TCP slow start.
6. How do we detect TCP errors?
   - check sum
   - random seed
