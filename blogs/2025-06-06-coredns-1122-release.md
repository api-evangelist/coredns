---
title: "CoreDNS-1.12.2 Release"
url: "https://coredns.io/2025/06/06/coredns-1.12.2-release/"
date: "Fri, 06 Jun 2025 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This release introduces significant improvements to plugin stability and extensibility. It adds multicluster support to the Kubernetes plugin, fallthrough support in the file plugin, and a new SetProxyOptions function for the forward plugin. Notably, the QUIC (DoQ) plugin now limits concurrent streams, improving performance under load. Several bug fixes and optimizations improve reliability across plugins, including rewrite, proxy, and metrics.
Brought to You By Ambrose Chua, Arthur Outhenin-Chalandre, Ben Kochie, Colden Cullen, Gleb Kogtev, Hirotaka Tagawa, Kevin Lyda, Manuel Rüger, Mark Mickan, Parfenov Ivan, skipper, vdbe, Viktor Oreshkin, Ville Vesilehto, Yannick Epstein, Yong Tang
