Database Management Systems (DBMSs) are foundational components
in modern software development, powering nearly every data-driven
application. Recent efforts have increasingly focused on detecting
logic bugs, beyond memory and performance issues, to ensure not
only availability but also operational correctness. However, prior
testing methods have targeted specific DBMSs and bug types, limiting
comprehensive approaches due to syntactic and semantic discrepancies
in SQL dialects across DBMSs.

We propose QueryHouse, a differential testing framework for discovering
logic bugs in a cross-DBMS context, leveraging a SQL transpiler and
LLMs. Specifically, we employ a customized transpiler to generate
adapted queries while resolving SQL discrepancies, and adopt a hybrid
mutation strategy that augments query mutation with an LLM to enhance
exploration. We evaluate QueryHouse on five widely used DBMSs—Oracle, MySQL,
PostgreSQL, SQLite, and MariaDB—and uncovered 11 previously unknown
bugs and 7 undocumented inconsistencies. Our experiments confirm
that the proposed methods improve query validity and exploration. We
believe QueryHouse enables scalable detection of core logic bugs, thereby
enhancing the robustness of DBMS software and their applications.
