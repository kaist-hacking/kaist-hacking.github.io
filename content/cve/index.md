---
title: Disclosed vulnerabilities

reading_time: false  # Show estimated reading time?
share: false  # Show social sharing links?
profile: false  # Show author profile?
comments: false  # Show comments?
---

{{<table "table">}}	

|Product     |CVE            | Description          | Lead  | Bounty |
|------------|---------------|----------------------|-------|--------|
|vm2         |CVE-2023-30547 |There exists a vulnerability in exception sanitization of vm2 for versions up to 3.9.16, allowing attackers to raise an unsanitized host exception inside handleException() which can be used to escape the sandbox and run arbitrary code in host context.|SeungHyun Lee||
|vm2         |CVE-2023-29199 | There exists a vulnerability in source code transformer (exception sanitization logic) of vm2 for versions up to 3.9.15, allowing attackers to bypass handleException() and leak unsanitized host exceptions which can be used to escape the sandbox and run arbitrary code in host context.|SeungHyun Lee||
|Firefox|CVE-2023-29548|A wrong lowering instruction in the ARM64 Ion compiler resulted in a wrong optimization result.|JunYoung Park|
|Chrome|CVE-2023-0696  | Type confusion in V8 in Google Chrome prior to 110.0.5481.77 allowed a remote attacker to potentially exploit heap corruption via a crafted HTML page. (Chromium security severity: High)|Haein Lee|$7,000|
|WebKit|CVE-2022-32923|A correctness issue in the JIT was addressed with improved checks. This issue is fixed in tvOS 16.1, iOS 15.7.1 and iPadOS 15.7.1, macOS Ventura 13, watchOS 9.1, Safari 16.1, iOS 16.1 and iPadOS 16. Processing maliciously crafted web content may disclose internal states of the app.|Wonyoung Jung||
|Samsung Exynos|CVE-2022-23425|Improper input validation in Exynos baseband prior to SMR Feb-2022 Release 1 allows attackers to send arbitrary NAS signaling messages with fake base station.|Eunsoo Kim, CheolJun Park|$14,760|
|NETGEAR R6700v3|PSV-2021-0304|Pre-Authentication Buffer Overflow in Some Routers|Insu Yun|$300|
{{</table>}}	
