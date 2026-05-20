---
title: "CoreDNS-1.8.5 Release"
url: "https://coredns.io/2021/09/10/coredns-1.8.5-release/"
date: "Fri, 10 Sep 2021 07:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This is a rather big release, we now share plugins among zones in the same server block, which should save memory. Various bug fixes in a bunch of plugins and not one, but two new plugins. A geoip plugin that can report where the query came from and a header plugin that allows you to fiddle with (some of) the header bits in a DNS message.
