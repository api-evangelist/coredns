---
title: "CoreDNS-1.14.6 Release"
url: "https://coredns.io/2026/07/10/coredns-1.14.6-release/"
date: "2026-07-10"
feed_url: "https://coredns.io/blog/index.xml"
---
This patch release focuses on fixing ARM and MIPS build issues introduced in v1.14.5 by downgrading the dd-trace-go dependency, while also including improvements to forwarding and secondary zone support. Brought to You By Filippo125 houyuwushang Immanuel Tikhonov Ville Vesilehto Yong Tang Noteworthy Changes core: Downgrade dd-trace-go to v2.8.2 (https://github.com/coredns/coredns/pull/8266) plugin/auto: Keep first matching zone file for duplicate origins (https://github.com/coredns/coredns/pull/8216) plugin/forward: Add source_address directive (https://github.com/coredns/coredns/pull/8011) pl
