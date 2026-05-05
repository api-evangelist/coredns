---
title: "CoreDNS-1.12.1 Release"
url: "https://coredns.io/2025/03/24/coredns-1.12.1-release/"
date: "Mon, 24 Mar 2025 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
In this release:
kubernetes: Revert recent change to only create PTR records for endpoints with hostname defined. forward: added option to return SERVFAIL immediately if all upstreams are unhealthy. Brought to You By Adrian Moisey, Arthur Outhenin-Chalandre, Bartosz Borkowski, Ben Kochie, Chris O&rsquo;Haver, Min Woo Kim, Puneet Loya, Rich, Viktor, momantech
Noteworthy Changes core: Increase CNAME lookup limit from 7 to 10 (https://github.com/coredns/coredns/pull/7153) plugin/kubernetes: Fix handling of pods having DeletionTimestamp set (https://github.
