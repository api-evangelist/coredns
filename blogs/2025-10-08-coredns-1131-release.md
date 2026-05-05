---
title: "CoreDNS-1.13.1 Release"
url: "https://coredns.io/2025/10/08/coredns-1.13.1-release/"
date: "Wed, 08 Oct 2025 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This release updates CoreDNS to Go 1.25.2 and golang.org/x/net v0.45.0 to address multiple high-severity CVEs. It also improves core performance by avoiding string concatenation in loops, and hardens the sign plugin by rejecting invalid UTF-8 tokens in dbfile.
Brought to You By Catena cyber Ville Vesilehto Yong Tang
Noteworthy Changes core: Avoid string concatenation in loops (https://github.com/coredns/coredns/pull/7572) core: Update golang to 1.25.2 and golang.org/x/net to v0.45.0 on CVE fixes (https://github.com/coredns/coredns/pull/7598) plugin/sign: Reject invalid UTF‑8 dbfile token (https://github.
