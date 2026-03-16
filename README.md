# CoreDNS (coredns)
CoreDNS is a CNCF graduated DNS server that serves as the default DNS for Kubernetes clusters. Built in Go with a plugin architecture, it provides flexible DNS-based service discovery, forwarding, caching, and integration with multiple backends.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/coredns/refs/heads/main/apis.yml)

## Scope
- **Type:** Index
- **Position:** Consumer
- **Access:** 3rd-Party

## Tags:
 - DNS, Service Discovery, Kubernetes, Networking, Cloud Native, Graduated

## Timestamps
- **Created:** 2026-03-16
- **Modified:** 2026-03-16

## APIs

### CoreDNS DNS Interface
CoreDNS implements the standard DNS protocol serving both UDP and TCP queries. In Kubernetes, it resolves service names to cluster IPs, headless services to pod IPs, and supports SRV records for port discovery.

**Human URL:** [https://coredns.io/manual/toc/](https://coredns.io/manual/toc/)

#### Tags:
 - DNS, Service Discovery, Kubernetes

#### Properties
- [Documentation](https://coredns.io/manual/toc/)

### CoreDNS Plugin API
The CoreDNS plugin framework allows extending DNS server functionality through a chain of plugins. External plugins can be written in Go to add custom DNS record sources, filtering, and middleware.

**Human URL:** [https://coredns.io/explugins/](https://coredns.io/explugins/)

#### Tags:
 - Plugins, Extensibility

#### Properties
- [Documentation](https://coredns.io/explugins/)

## Common Properties
- [Documentation](https://coredns.io/manual/toc/)
- [GitHub](https://github.com/coredns)
- [Blog](https://coredns.io/blog/)

## Maintainers
**FN:** Kin Lane
**Email:** kin@apievangelist.com
