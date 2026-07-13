---
title: "redis_cache"
url: "https://coredns.io/explugins/redis_cache/"
date: "2026-05-11"
feed_url: "https://coredns.io/explugins/index.xml"
---
Description redis_cache stores DNS responses in a shared Redis-compatible backend (Redis, Valkey, or any RESP-protocol server) so that multiple CoreDNS instances can amortize upstream lookups across the fleet — for example several pods in a Kubernetes cluster, or a fleet of node-local-dns daemons. It is intended to sit behind the built-in cache plugin, which stays as the L1 (in-process) cache; redis_cache is the L2 (networked) cache. If the Redis backend is unreachable the plugin becomes a noop and lookups continue to flow through the rest of the chain.
