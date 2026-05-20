---
title: "CoreDNS-1.3.1 Release"
url: "https://coredns.io/2019/01/13/coredns-1.3.1-release/"
date: "Sun, 13 Jan 2019 15:00:29 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
We are pleased to announce the release of CoreDNS-1.3.1! This is a fairly small release that allows us to announce some backwards incompatible changes in the next (1.4.0) release: The upstream directive used in various plugin will start to default to the coredns process itself. This allow those resolutions to take advantage of other plugins (i.e. caching).
