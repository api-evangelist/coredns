---
title: "CoreDNS-1.13.0 Release"
url: "https://coredns.io/2025/10/05/coredns-1.13.0-release/"
date: "Sun, 05 Oct 2025 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This release introduces a new Nomad plugin for integrating CoreDNS with HashiCorp Nomad. It also fixes major Corefile issues on infinite loops and import cycles, improves shutdown handling, normalizes core panics, addresses data races in the file plugin, enforces gRPC size limits, adjusts forward failover behavior, as well as prevents reload deadlocks. Brought to You By Fitz_dev Ilya Kulakov Olli Janatuinen Ville Vesilehto Yong Tang Noteworthy Changes core: Export timeout values in dnsserver.
