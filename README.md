# MongoDB_Redis_Geospatial

Compared MongoDB and Redis for geospatial data processing to evaluate performance and cost trade-offs for large-scale spatial applications, resulting in clear use-case recommendations (Redis for real-time low-latency needs, MongoDB for complex queries).

Prepared and optimized OpenStreetMap (OSM) datasets for MongoDB and Redis compatibility, enabling accurate benchmarking of 1.8M records, with Redis achieving 12x faster match queries (90ms vs. MongoDB’s 1081ms).

Designed and executed geospatial queries (proximity searches, match queries) to test database performance, resulting in MongoDB outperforming Redis in geospatial queries (4ms vs. 43ms) due to native 2D indexing.

Implemented automated backup/restore pipelines using mongodump and Redis .rdb files, ensuring data reliability and reducing recovery time during failures.

Benchmarked scalability and cost efficiency across Azure VMs, revealing Redis’s 80,000+ TPS (transactions/second) at scale but 70x higher cost-per-million transactions vs. MongoDB for large datasets.

Identified Redis’s limitations in community support and setup complexity, leading to documented workarounds for RedisJSON module integration and Lua script challenges.

Recommended database choices based on findings: Redis for real-time caching/gaming (low latency), MongoDB for cost-effective geospatial analytics with complex aggregations.
