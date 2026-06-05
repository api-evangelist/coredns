# CoreDNS (coredns)

CoreDNS is a CNCF graduated DNS server written in Go that serves as the default DNS service for Kubernetes clusters. It is flexible and extensible through a plugin architecture, supporting DNS-based service discovery, forwarding, caching, and integration with etcd, Kubernetes, and other backends. CoreDNS can serve as an authoritative DNS server or a recursive resolver, with HTTP plugins exposing health, readiness, and Prometheus metrics endpoints for Kubernetes operations.

**APIs.json:** [https://coredns.io](https://coredns.io)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** Public

## Tags

- Apache 2.0
- Cloud Native
- CNCF
- DNS
- Go
- Graduated
- Kubernetes
- Networking
- Open Source
- Plugins
- Prometheus
- Service Discovery

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-19

## APIs

### CoreDNS DNS Interface

CoreDNS implements the standard DNS protocol (RFC 1035) serving both UDP and TCP queries. In Kubernetes, it resolves service names to cluster IPs, headless services to pod IPs, and supports SRV records for port discovery. The Kubernetes plugin watches the API server for service and endpoint changes to keep DNS records current. Additional protocol bindings include DNS-over-TLS (DoT), DNS-over-HTTPS (DoH), DNS-over-QUIC (DoQ), and gRPC.

- **Human URL:** [https://coredns.io/manual/toc/](https://coredns.io/manual/toc/)

#### Tags

- DNS
- DoH
- DoQ
- DoT
- Kubernetes
- Service Discovery

#### Properties

- [Documentation](https://coredns.io/manual/toc/)
- [Postman Collection](collections/coredns-health.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coredns-health.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/coredns-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coredns-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CoreDNS Plugin API

The CoreDNS plugin framework allows extending DNS server functionality through a chain of plugins defined in the Corefile configuration. External plugins can be written in Go to add custom DNS record sources, filtering, metrics, and middleware. Each plugin implements the Handler interface to process DNS requests.

- **Human URL:** [https://coredns.io/explugins/](https://coredns.io/explugins/)

#### Tags

- Extensibility
- Plugins

#### Properties

- [Documentation](https://coredns.io/explugins/)
- [Reference](https://coredns.io/manual/plugins/)
- [Postman Collection](collections/coredns-health.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coredns-health.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/coredns-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coredns-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### CoreDNS Health API

The CoreDNS health plugin exposes HTTP /health and /ready endpoints on port 8080 by default. It reports the overall health and readiness of the CoreDNS process and is used by Kubernetes liveness and readiness probes to determine if the DNS server is operational.

- **Human URL:** [https://coredns.io/plugins/health/](https://coredns.io/plugins/health/)
- **Base URL:** `http://localhost:8080`

#### Tags

- Health Check
- Kubernetes
- Observability
- Readiness

#### Properties

- [Documentation](https://coredns.io/plugins/health/)
- [Ready Documentation](https://coredns.io/plugins/ready/)
- [OpenAPI](openapi/coredns-health-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/coredns-health.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coredns-health.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Rules](rules/coredns-health-rules.yml)
- [Capabilities](capabilities/coredns-health-capabilities.yml)

### CoreDNS Metrics API

The CoreDNS prometheus plugin exposes a Prometheus-compatible metrics endpoint at /metrics on port 9153. It provides DNS request counters, response size histograms, latency distributions, and build information metrics for monitoring CoreDNS performance and behavior.

- **Human URL:** [https://coredns.io/plugins/metrics/](https://coredns.io/plugins/metrics/)
- **Base URL:** `http://localhost:9153`

#### Tags

- Metrics
- Monitoring
- Observability
- Prometheus

#### Properties

- [Documentation](https://coredns.io/plugins/metrics/)
- [OpenAPI](openapi/coredns-metrics-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/coredns-metrics.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/coredns-metrics.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Rules](rules/coredns-metrics-rules.yml)
- [Capabilities](capabilities/coredns-metrics-capabilities.yml)

## Common Properties

- [JSON Schema](json-schema/coredns-corefile-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/coredns-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Vocabulary](vocabulary/coredns-vocabulary.yml)
- [Website](https://coredns.io/)
- [Documentation](https://coredns.io/manual/toc/)
- [Getting Started](https://coredns.io/2017/07/24/quick-start/)
- [GitHub Organization](https://github.com/coredns)
- [GitHub Repository](https://github.com/coredns/coredns)
- [Plugins](https://coredns.io/plugins/)
- [External Plugins](https://coredns.io/explugins/)
- [Blog](https://coredns.io/blog/)
- [Changelog](https://github.com/coredns/coredns/releases)
- [Community](https://slack.cncf.io/)
- [License](https://github.com/coredns/coredns/blob/master/LICENSE)
- [C N C F](https://www.cncf.io/projects/coredns/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
