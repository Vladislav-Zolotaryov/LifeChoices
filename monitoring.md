# Solutions
* ELK - heavy, robust 
* Datadog - pricy, cloud, robust
* Loki Stack - lightweight, lacks features

# Metrics
* OS - CPU, Memory, Storage
* JVM - Heap, Non-Heap, GC size, GC time
* Kubernetes - Pods, Pod crashes
* Web applications - request rates and response times for endpoints, DB connections in pool, thread/virtual thread counts
* DB - query timings, total connections, transation rate, Disk Read/Write speeds, VACUUM times for PostgreSQL


# Log Collectors
fluent-bit - efficient, mature
Promtail - if you use Loki Stack and single tenant

# Observability Collectors (Metrics, Logs, APM)
vector - ultra efficient, less mature (by DataDog)
