---
title: "CoreDNS-1.14.2 Release"
url: "https://coredns.io/2026/03/06/coredns-1.14.2-release/"
date: "Fri, 06 Mar 2026 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This release adds the new proxyproto plugin to support Proxy Protocol and preserve client IPs behind load balancers. It also includes enhancements such as improved DNS logging metadata and stronger randomness for loop detection (CVE-2026-26018), along with several bug fixes including TLS+IPv6 forwarding, improved CNAME handling and rewriting, allowing jitter disabling, prevention of an ACL bypass (CVE-2026-26017), and a Kubernetes plugin crash fix. In addition, the release updates the build to Go 1.
