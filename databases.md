 * PostgreSQL - best all-round for larger loads (Maybe try to replace with AlloyDB Omni)
 * MariaDB - best developer friendly RDBMS
 * MongoDB - best read optimized NoSQL for JSON documents
 * Couchbase - best allround NoSQL DB
 * CockroachDB - probably best horizontal scaling RDBMS
 * ScyllaDB - probably good NoSQL for readiness and scaling, faster Cassandra alternative
 * Cassandra - best write optimized, columnar NoSQL
 * SurrealDB - multi-model database
 * Neo4J - best graph DB
 * Redis - most mature key-value with all-rounder features support 
 * Hazelcast - embeddable java written key-value with good scaling capabilities
 * SurrealDB - Rust based multi-model DB

For small scale datasets when your data size and request rate can be handled by a single node DB, the best choices are:
 * PostgreSQL (the only choice if you need OLTP)
 * MongoDB
 * Couchbase

For large scale datasets with multiple nodes and high request loads, the best choices are:
 * ScyllaDB
 * Couchbase

https://benchant.com/
