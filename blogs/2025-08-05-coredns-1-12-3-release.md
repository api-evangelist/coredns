---
title: "CoreDNS-1.12.3 Release"
url: "https://coredns.io/2025/08/05/coredns-1.12.3-release/"
date: "Tue, 05 Aug 2025 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This release improves plugin reliability and standards compliance, adding startup timeout to the Kubernetes plugin, fallthrough to gRPC, and EDNS0 unset to rewrite. The file plugin now preserves SRV record case per RFC 6763, route53 is updated to AWS SDK v2, and multiple race conditions in cache and connection handling in forward are fixed. Brought to You By blakebarnett Brennan Kinney Cameron Steel Dave Brown Dennis Simmons Guillaume Jacquet harshith-2411-2002 houpo-bob Oleg Guba Sebastian Mayr Stephen Kitt Syed Azeez Ville Vesilehto Yong Tang Yoofi Quansah
