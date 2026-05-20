---
title: "CoreDNS-1.4.0 Release"
url: "https://coredns.io/2019/03/03/coredns-1.4.0-release/"
date: "Sun, 03 Mar 2019 09:04:07 +0000"
author: ""
feed_url: "https://coredns.io/blog/index.xml"
---
We are pleased to announce the release of CoreDNS-1.4.0! Our first release after we became a graduated project in CNCF. Deprecation notice for the next release: auto will deprecate TIMEOUT and recommends the use of RELOAD (2516). auto and file will deprecate NO_RELOAD and recommends the use of RELOAD set to 0 (2536). health will revert back to report process level health without plugin status.
