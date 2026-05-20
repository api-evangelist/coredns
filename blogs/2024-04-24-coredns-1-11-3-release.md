---
title: "CoreDNS-1.11.3 Release"
url: "https://coredns.io/2024/04/24/coredns-1.11.3-release/"
date: "Wed, 24 Apr 2024 16:57:00 -0400"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This release contains some new features, bug fixes, and package updates. Because of the deployment issues with the previous release, all changed features from 1.11.2 have been included in this release. New features include: When the forward plugin receives a malformed upstream response that overflows, it will now send an empty response to the client with the truncated (TC) bit set to prompt the client to retry over TCP.
