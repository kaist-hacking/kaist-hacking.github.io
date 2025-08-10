---
# An instance of the Blank widget.
# Documentation: https://sourcethemes.com/academic/docs/page-builder/
widget: blank

# Activate this widget? true/false
active: true

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 15

title: News

---
* [08/09/2025] Team Atlanta wins [AIxCC](https://aicyberchallenge.com/)!
* [05/30/2025] LLFuzz is accepted to [USENIX Security '25](https://www.ieee-security.org/TC/SEC2025/index.html)!
* [04/28/2025] FirmState is accepted to [WiSec '25](https://wisec2025.gmu.edu/)!
* [03/31/2025] CPMM-Exploiter is accepted to [ISSTA '25](https://conf.researchr.org/home/issta-2025)!
* [12/30/2024] Security analysis of mandatory security software in South Korea is accepted to [USENIX Security '25](https://www.ieee-security.org/TC/SEC2025/index.html)!
* [12/19/2024] FIBLE is accepted to [OOPSLA '25](https://2025.splashcon.org/track/OOPSLA)!
* [09/10/2024] RGFuzz is accepted to [IEEE S&P '25](https://www.ieee-security.org/TC/SP2025/index.html)!
* [08/11/2024] Team Atlanta proceeds to [the AIxCC final](https://aicyberchallenge.com/)!
* [03/22/2024] Seunghyun won [Pwn2Own 2024](https://www.zerodayinitiative.com/blog/2024/3/21/pwn2own-vancouver-2024-day-two-results) by exploiting Google Chrome and Microsoft Edge ($145K)!
* [01/25/2024] $10K Bug Bounty from Google v8CTF (V8/CVE-2023-6702).
* [10/25/2023] We got 2nd place in [cyber security challenge 2023](https://sec-challenge.kr/main)!
* [10/04/2023] $67K Bug Bounty from Google kernelCTF (Linux/CVE-2023-3390).
* [07/17/2023] QSYM got a Frontiers of Science Award from [ICSB](https://www.icbs.cn/)!
* [06/06/2023] BaseComp is accepted to [Usenix Security'23](https://www.usenix.org/conference/usenixsecurity23)!
* [01/19/2023] $7K Bug Bounty from Google (V8/CVE-2023-0696).
* [11/11/2022] QueryX is accepted to [IEEE
    S&P'23](https://www.ieee-security.org/TC/SP2023/index.html)!
* [11/04/2022] ScaleTrust is accepted to [ToN'22](https://ieeexplore.ieee.org/xpl/RecentIssue.jsp?punumber=90)!
* [06/11/2022] FuzzCoin is accepted to [RAID'22](https://raid2022.cs.ucy.ac.cy/index.html)!
* [09/04/2021] DoLTEst is conditionally accepted to [Usenix Security'22](https://www.usenix.org/conference/usenixsecurity22)!
* [07/21/2021] HardsHeap is conditionally accepted to [CCS'21](https://www.sigsac.org/ccs/CCS2021/)! 


<script>
    document.addEventListener("DOMContentLoaded", function () {
        const section = document.querySelector("#news");
        if (!section) return;

        const list = section.querySelector("ul");
        if (!list) return;

        const items = list.querySelectorAll("li");
        const moreLink = document.createElement("a");
        moreLink.href = "#";
        moreLink.textContent = "Show more";
        moreLink.style.marginTop = "10px";
        moreLink.style.display = "block";
        moreLink.style.cursor = "pointer";
        moreLink.style.textDecoration = "underline";

        let isExpanded = false;

        items.forEach((item, index) => {
            if (index >= 10) {
                item.style.display = "none";
            }
        });

        moreLink.addEventListener("click", (e) => {
            e.preventDefault();
            isExpanded = !isExpanded;
            items.forEach((item, index) => {
                if (index >= 10) {
                    item.style.display = isExpanded ? "block" : "none";
                }
            });
            moreLink.textContent = isExpanded ? "Show less" : "Show more";
        });
        list.parentNode.insertBefore(moreLink, list.nextSibling);
    });
</script>
