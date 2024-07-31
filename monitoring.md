# Solutions
* ELK - resource heavy, robust, lacks features
* Datadog - pricy, cloud only, robust
* Grafana LGTM - lightweight, lacks features
* SigNoz - maturing simple observability stack
* DynaTrace - pricy, cloud only, robust solution
* New Relic - pricy, cloud only, users complain about unstable pricing model and unexpected changes in billing
* AppDynamics - strange product by Cisco

# Metrics
* OS - CPU, Memory, Storage
* JVM - Heap, Non-Heap, GC size, GC time
* Kubernetes - Pods, Pod crashes
* Web applications - request rates and response times for endpoints, DB connections in pool, thread/virtual thread counts
* DB - query timings, total connections, transation rate, Disk Read/Write speeds, VACUUM times for PostgreSQL
* eBPF - linux kernel level metrics (Grafana Beyla one of solutions)

# Log Collectors
* fluent-bit - efficient, mature
* Promtail - if you use Loki Stack and single tenant

# Observability Collectors (Metrics, Logs, APM)
vector - ultra efficient, less mature (by DataDog)
