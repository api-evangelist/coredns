# CoreDNS (coredns)

CoreDNS is a CNCF graduated DNS server written in Go that serves as the default DNS service for Kubernetes clusters. It is flexible and extensible through a plugin architecture, supporting DNS-based service discovery, forwarding, caching, and integration with etcd, Kubernetes, and other backends. CoreDNS can serve as an authoritative DNS server or a recursive resolver.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/coredns/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** Public
- **x-type:** opensource

## Tags

- Apache 2.0, Cloud Native, CNCF, DNS, Go, Graduated, Kubernetes, Networking, Open Source, Plugins, Prometheus, Service Discovery

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-28

## APIs

### CoreDNS DNS Interface

Standard DNS protocol (RFC 1035) over UDP/TCP, with bindings for DNS-over-TLS (DoT), DNS-over-HTTPS (DoH), DNS-over-QUIC (DoQ), and gRPC.

- [Documentation](https://coredns.io/manual/toc/)

### CoreDNS Plugin API

Plugin framework for extending DNS server functionality through a chain of plugins defined in the Corefile configuration.

- [Documentation](https://coredns.io/explugins/)
- [Reference](https://coredns.io/manual/plugins/)

### CoreDNS Health API

HTTP /health and /ready endpoints exposed on port 8080 by default for Kubernetes liveness and readiness probes.

- [Documentation](https://coredns.io/plugins/health/)
- [OpenAPI](openapi/coredns-health-openapi.yml)
- [Rules](rules/coredns-health-rules.yml)
- [Capabilities](capabilities/coredns-health-capabilities.yml)

### CoreDNS Metrics API

Prometheus-compatible metrics endpoint at /metrics on port 9153 with DNS request counters, response size histograms, latency distributions, and build information.

- [Documentation](https://coredns.io/plugins/metrics/)
- [OpenAPI](openapi/coredns-metrics-openapi.yml)
- [Rules](rules/coredns-metrics-rules.yml)
- [Capabilities](capabilities/coredns-metrics-capabilities.yml)

## Common Properties

- [Website](https://coredns.io/)
- [Documentation](https://coredns.io/manual/toc/)
- [Getting Started](https://coredns.io/2017/07/24/quick-start/)
- [GitHub](https://github.com/coredns/coredns)
- [Plugins](https://coredns.io/plugins/)
- [External Plugins](https://coredns.io/explugins/)
- [Vocabulary](vocabulary/coredns-vocabulary.yml)
- [JSON-LD Context](json-ld/coredns-context.jsonld)
- [Corefile JSON Schema](json-schema/coredns-corefile-schema.json)
- [CNCF Project Page](https://www.cncf.io/projects/coredns/)
- [License (Apache 2.0)](https://github.com/coredns/coredns/blob/master/LICENSE)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
