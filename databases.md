Parameters to consider:

* Vertical Scaling
* Horizontal Scaling (Clustering/Sharding Protocol and Topology) 
* Storage Solution (B-Tree (Locking, WAL, Copy-On-Write MVCC), LSM)
* Distributed Transactions (2PC, Paxos, Raft)
* Indexing (Global, Local)
* OLTP vs OLAP
* Community Edition trade-offs
* Paid Edition Price
* TCO (CPU, RAM, Storage, Traffic, License, Maintenance costs)
* Developer Experience (Can spin up locally, drivers are available for language, usage is simple enough to compherend for everyone in the team)
* Maintainer Experience (Replica Repairs, Vaccuums)
* Analytics Queries (Parallel requests, Map-Reduce)
* Materialized Views (Automatic, overhead cost)
* Partitioning (and Clustering, pre-sorting)
* Timeseries Queries (Ability to show data analytics for group of entries by time 1, 7, 30, 90, 180, 365 days)
* Audit logs
* TTLs support
* Security (Per Instance, Per logical DB, Per Schema, Per Table, Per Row)
* Encryption (level of encryption, at rest, e2e, etc)
* Compaction
* Multi-tenancy
* User Defined Functions
* CRON tasks
* JSON Support
* Backup/Restore tools
* CDC support
* External data source support (importing data from S3, linking between databases/clusters)
* Ability to move databases/keyspaces between databases/clusters
* High availability
* Cluster partitioning scenario handling
* Datacenter and rack awareness
* Schema and data migration
* Metrics (Ability to export metrics)
* Tracing (Support for APM)
* Managment tools (easy tools to look at data and state)
* Serverlesness (automatic scaling)


Databases:
 
 * PostgreSQL - best all-round for larger loads (Maybe try to replace with AlloyDB Omni at scale), reads can scale to a degree by using read-replicas, other possible clustering solutions are Citus (2PC) and AWS Aurora or Greemplum, Timescale for OLAP
 * Neon - Serverless PostgreSQL compliant
 * MariaDB - best developer friendly RDBMS can be master-master clustered using Percona or Galera
 * MongoDB - best read optimized NoSQL for JSON documents
 * Couchbase - best allround NoSQL DB
 * CockroachDB - probably best horizontal scaling RDBMS
 * ScyllaDB - probably good NoSQL for readiness and scaling, faster Cassandra alternative, Raft
 * Cassandra - best write optimized, columnar NoSQL, Paxos
 * SurrealDB - multi-model database
 * Neo4J - best graph DB
 * Redis - most mature key-value with all-rounder features support (No longer open source, replace with KeyDB)
 * Hazelcast - embeddable java written key-value with good scaling capabilities
 * Aerospike - multi-model key-value oriented, new product, needs research
 * DragonflyDB - Theoretically fastest key-value store
 * RethinkDB - open-source database for the realtime web
 * RavenDB - multi-master, Raft
 * LevelDB (RocksDB)

For small scale datasets when your data size and request rate can be handled by a single node DB, the best choices are:
 * PostgreSQL (the only choice if you need OLTP)
 * MongoDB
 * Couchbase

For large scale datasets with multiple nodes and high request loads, the best choices are:
 * ScyllaDB
 * Couchbase

https://benchant.com/
