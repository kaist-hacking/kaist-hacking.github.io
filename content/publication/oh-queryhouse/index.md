---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'QueryHouse: Cross-DBMS Differential Testing with LLM and Query Transpilation'
subtitle: ''
summary: ''
authors:
- Seoyeon Oh
- Juhyun Song
- Jaemin Park
- Kwanghee Lee
- Minae Hyeon
- Minji Kim
- Sehyuk Ka
- Gwangwun Jung
- Brian Pak
- Insu Yun
tags: []
categories: []
date: '2026-09-01'
lastmod: 2026-10-27T17:36:40+09:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2026-10-27T08:36:39.955821Z'
publication_types:
- '0'
abstract: "Database Management Systems (DBMSs) are foundational components\nin modern\
  \ software development, powering nearly every data-driven\napplication. Recent efforts\
  \ have increasingly focused on detecting\nlogic bugs, beyond memory and performance\
  \ issues, to ensure not\nonly availability but also operational correctness. However,\
  \ prior\ntesting methods have targeted specific DBMSs and bug types, limiting\n\
  comprehensive approaches due to syntactic and semantic discrepancies\nin SQL dialects\
  \ across DBMSs.\n\nWe propose QueryHouse, a differential testing framework for discovering\n\
  logic bugs in a cross-DBMS context, leveraging a SQL transpiler and\nLLMs. Specifically,\
  \ we employ a customized transpiler to generate\nadapted queries while resolving\
  \ SQL discrepancies, and adopt a hybrid\nmutation strategy that augments query mutation\
  \ with an LLM to enhance\nexploration. We evaluate QueryHouse on five widely used\
  \ DBMSs—Oracle, MySQL,\nPostgreSQL, SQLite, and MariaDB—and uncovered 11 previously\
  \ unknown\nbugs and 7 undocumented inconsistencies. Our experiments confirm\nthat\
  \ the proposed methods improve query validity and exploration. We\nbelieve QueryHouse\
  \ enables scalable detection of core logic bugs, thereby\nenhancing the robustness\
  \ of DBMS software and their applications.\n"
publication: '*Proceedings of the 31st European Symposium on Research in Computer
  Security (ESORICS)*'
url_slides: pubs/2026/oh:queryhouse-slides.pdf
url_paper: pubs/2026/oh:queryhouse.pdf
award: '**Best Paper Award Runner-up**'
---
