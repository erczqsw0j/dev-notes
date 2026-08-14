# Go Microservices Checklist

Quick sanity list before shipping a new service or endpoint.

- [ ] Context propagation (timeouts, cancellation)
- [ ] Structured logging (request ID, service, method)
- [ ] Metrics: latency, errors, throughput
- [ ] Graceful shutdown (signal handling)
- [ ] Retry with backoff for downstream calls
- [ ] Circuit breaker for critical dependencies
- [ ] Config via env vars, not hardcoded
- [ ] Health and readiness endpoints separate
- [ ] Panic recovery middleware
- [ ] DB connection pooling and max idle time
- [ ] Idempotency keys for writes
- [ ] Proper HTTP status codes and error bodies

Add new items as we learn from incidents.