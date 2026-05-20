---
title: "CoreDNS-1.5.1 Release"
url: "https://coredns.io/2019/06/26/coredns-1.5.1-release/"
date: "Wed, 26 Jun 2019 13:54:47 +0100"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
The CoreDNS team has released CoreDNS-1.5.1. Various bugfixes, better documentation and cleanups. The -cpu flag is somewhat redundant (cgroups/systemd/GOMAXPROCS are better ways to deal with this) and we want to remove it; if you depend on it in some way please voice that in this PR otherwise we’ll remove it in the next release.
