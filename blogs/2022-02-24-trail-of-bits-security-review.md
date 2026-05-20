---
title: "Trail Of Bits Security Review"
url: "https://coredns.io/2022/02/24/trail-of-bits-security-review/"
date: "Thu, 24 Feb 2022 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
Trail of Bits (https://trailofbits.com) conducted a security review and threat model of CoreDNS. Quoting from the security review summary: “The audit uncovered one high-severity issue (TOB-CDNS-8) concerning a bug that could lead to cache poisoning attacks. The majority of the other issues are of informational or low severity; these include several resulting from insufficient data validation, specifically from assumptions about the data processed by various functions, which we discovered by running fuzzing harnesses.
