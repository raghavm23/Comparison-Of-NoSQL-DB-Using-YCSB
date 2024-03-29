# MongoDB vs Cassandra (performance comparison)

Modern day applications create exceptionally large volumes of ever increasing data and ever changing data types. Hence it is not feasible to store such data in the conventional relational databases as they are not optimised for horizontal scaling. This paves the way for NoSQL databases and in this project we compare the architecture and performance of two such NoSQL databases ie. MongoDB and Cassandra.

## Yahoo! Cloud Service Benchmark Framework
Developed by [Brian Frank Cooper](https://github.com/brianfrankcooper/YCSB)

The YCSB tool consists of a ycsb-client which generates the workload and the defined workloads which are the scenarios to be executed by the client.

## Performance Test Plan
**Two** NoSQL DB compared- MongoDB and Cassandra

**Two** predefined workloads A & B are chosen for the performance testing
Workload A : Update heavy workload – 50/50 reads and writes
Workload B : Read mostly workload – 95/5 reads and writes

**Five** different number of operations chosen for testing are 100000, 250000, 500000, 750000 and 1000000**

**Three** times each test is performed for accurate and consistent results

**--60 total iterations--**

## Conclusion
**MongoDB** provides **superior** performance than **Cassandra** in my testing scenarios. The **overall throughput** is much higher for **MongoDB**, sometimes attaining more than **5x of Cassandra**. MongoDB also exhibits much lower latency in both the workloads across all operation counts.
