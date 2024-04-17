# CAP Theorem Explained with Examples

## What is the CAP Theorem?

The CAP theorem, also known as Brewer's theorem, states that in a distributed data store, it is impossible to simultaneously achieve all three of the following properties: Consistency, Availability, and Partition tolerance.

### Consistency

Consistency refers to all nodes in a distributed system having the same data at the same time. When a write operation is completed, all subsequent read operations should return the updated data.

### Availability

Availability ensures that every request made to the distributed system receives a response, either success or failure. The system remains operational even in the presence of failures.

### Partition Tolerance

Partition tolerance means that the distributed system continues to operate despite network partitions (communication failures) between nodes.

## Examples

### CP Systems (Consistency and Partition Tolerance)

In CP systems, consistency and partition tolerance are prioritized over availability. These systems guarantee that all nodes have consistent data and can tolerate network partitions, but they may become temporarily unavailable in the event of a network partition.

**Example**: Relational databases like PostgreSQL and Oracle prioritize consistency and partition tolerance. During a network partition, these databases ensure that all nodes have consistent data, but some nodes may become unavailable until the partition is resolved.

### AP Systems (Availability and Partition Tolerance)

In AP systems, availability and partition tolerance are prioritized over consistency. These systems ensure that every request receives a response and can tolerate network partitions, but they may return stale or divergent data.

**Example**: NoSQL databases like Cassandra and MongoDB prioritize availability and partition tolerance. During a network partition, these databases remain operational and continue to serve requests, even if some nodes have divergent data. Consistency may be sacrificed temporarily to maintain availability.

### CP Systems with Eventual Consistency

Some systems aim to achieve eventual consistency, meaning that all nodes will eventually converge to a consistent state after a period of time, even in the presence of network partitions.

**Example**: Dynamo-style databases like Amazon DynamoDB prioritize consistency and partition tolerance but offer eventual consistency. These databases ensure that all nodes eventually converge to a consistent state, but there may be temporary inconsistencies during network partitions.

## Conclusion

The CAP theorem highlights the trade-offs involved in designing distributed systems. While it is impossible to achieve all three properties simultaneously, understanding the implications of these trade-offs helps in selecting the appropriate consistency model based on the requirements of the application.
