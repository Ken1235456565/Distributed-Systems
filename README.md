####  reference
[《Distributed Systems 》](http://nil.csail.mit.edu/6.824/2016/schedule.html)
+ [《大规模分布式存储系统》](https://book.douban.com/subject/25723658/)
+ [《分布式系统原理介绍》](http://pan.baidu.com/s/1geU1XAz)
+ [awesome-distributed-systems](https://github.com/kevinxhuang/awesome-distributed-systems)
+ [一名分布式存储工程师的技能树是怎样的？](https://www.zhihu.com/question/43687427/answer/96306564)
+ [袖珍分布式系统](http://www.jianshu.com/c/0cf64976a481)

MIT 6.824: Distributed Systems Labs
This repository contains the implementation and translated documentation for the labs associated with the MIT 6.824 Distributed Systems course. The project focuses on building core distributed systems components using the Go programming language.

Project Structure
The project is organized into several lab modules, each addressing a fundamental challenge in distributed computing:

MapReduce: A system for processing large datasets in parallel across a cluster. The implementation includes the Master and Worker logic, handling task assignment and fault tolerance.

Raft Consensus Algorithm: A replicated state machine protocol designed for manageability. It ensures that a cluster of nodes can agree on a shared state even in the presence of failures.

Key/Value Service:

kvraft: A fault-tolerant key/value storage service built on top of the Raft consensus algorithm.

kvpaxos: An alternative implementation of a key/value service utilizing the Paxos protocol.

Sharded Storage:

ShardMaster: A configuration service that manages the assignment of shards to replica groups.

ShardKV: A sharded key/value storage system that partitions data across multiple replica groups for scalability.

Primary-Backup Service: A simple replication system where a primary server handles requests and synchronizes state with a backup.

Infrastructure & Tools
LabRPC: A customized RPC (Remote Procedure Call) library used to simulate network behavior, including delays, packet loss, and reordering, to test the robustness of the distributed algorithms.

Testing Framework: Each module includes a comprehensive suite of tests to verify correctness under various failure scenarios.

Utility Scripts: Shell scripts are provided to automate the execution of MapReduce jobs and integration tests.

Development Environment
Language: Go (Golang).

Build System: Makefile for managing compilation and testing workflows.

Platform: Developed and tested on macOS/Linux environments.
