# CoreDNS (coredns)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
