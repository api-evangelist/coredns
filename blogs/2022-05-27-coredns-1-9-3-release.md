---
title: "CoreDNS-1.9.3 Release"
url: "https://coredns.io/2022/05/27/coredns-1.9.3-release/"
date: "Fri, 27 May 2022 00:00:00 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
This is a release with a focus on security (CVE-2022-27191 and CVE-2022-28948) fixes. Additionally, several feature enhancements and bug fixes have been added. Brought to You By Chris O’Haver, lobshunter, Naveen, Radim Hatlapatka, RetoHaslerMGB, Tintin, Yong Tang Noteworthy Changes core: update gopkg.in/yaml.v3 to fix CVE-2022-28948 (https://github.com/coredns/coredns/pull/5408) core: update golang.org/x/crypto to fix CVE-2022-27191 (https://github.com/coredns/coredns/pull/5407) plugin/acl: adding a check to parse out zone info (https://github.com/coredns/coredns/pull/5387) plugin/dnstap:…
