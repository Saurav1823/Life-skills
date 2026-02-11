# Investigating Caching Approaches to Resolve Performance Issues

## Introduction

After joining the new project, it was observed that the application is facing performance and scalability issues due to repeated database queries and increased response time. The system frequently fetches the same data from the database, which increases server load and affects overall performance. As traffic grows, this problem can become more critical and may lead to system instability. To address these challenges, different caching approaches were analyzed as a potential solution to improve performance and support scalability.

## Caching Solution

Caching is a technique that stores frequently accessed data in a fast memory layer so that future requests can be served quickly without repeatedly querying the database. This reduces latency, decreases database load, and improves overall system efficiency. Instead of processing the same request multiple times, the application first checks whether the required data is available in the cache. If the data is found, it is returned immediately. If not, the application fetches it from the database and stores it in the cache for future use.

The following caching approaches were considered:

* Application-level caching using in-memory storage  
* Distributed caching using Redis or Memcached  
* Client-side caching for static resources  
* CDN caching for faster global content delivery  

Application-level caching is simple to implement but is limited to a single server instance. Distributed caching provides a shared in-memory store that can be accessed by multiple application servers, making it suitable for horizontally scalable systems. Client-side and CDN caching reduce network latency and improve the delivery speed of static assets such as images, stylesheets, and scripts.

Among these options, distributed caching using Redis with the Cache-Aside strategy is the most suitable approach. It allows multiple servers to access a shared cache, reduces database load, and improves response time. Proper Time To Live configuration and cache invalidation policies must be implemented carefully to maintain data consistency and avoid stale data issues.

By implementing caching strategically, the project can achieve improved performance, better scalability, reduced infrastructure costs, and enhanced user experience.

## References

* https://redis.io/docs/latest/develop/get-started/data-types/  
* https://aws.amazon.com/caching/  
* https://www.cloudflare.com/learning/cdn/what-is-caching/  
* https://www.geeksforgeeks.org/caching-system-design-concept/  
