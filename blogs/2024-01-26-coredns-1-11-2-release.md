---
title: "CoreDNS-1.11.2 Release"
url: "https://coredns.io/2024/01/26/coredns-1.11.2-release/"
date: "Fri, 26 Jan 2024 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This release contains some new features, bug fixes, and package updates. New features include: When the forward plugin receives a malformed upstream response that overflows, it will now send an empty response to the client with the truncated (TC) bit set to prompt the client to retry over TCP. The rewrite plugin can now rewrite response codes.
