# Java specialization skill map

Every learner completes the Java SE checks below. Team submissions supply the code; each learner explains, changes and tests an identifiable part unaided. The application sequence has three anchors (lets-play, angul-it, 01blog) and a mandatory systems project (java-localserver). Its separate Platform graph branch lets the cohort schedule it after the piscine.

## What counts as evidence

Scope each issue with four fields: **skill**, **first learner-owned implementation**, **individual demonstration**, **later work eligible for AI**. Link a reviewed PR or audit record before delegating repetition. A learner who cannot handle the variation gets another attempt on the same skill. Give learners different variations on a shared codebase. A passing tester, a team demo or an AI-generated explanation alone supplies insufficient individual evidence. Platform rules govern official submissions.

## Required Java API checks for every learner

These are cohort review choices. The first two columns distinguish what the learner has encountered from where to assess transfer. Select the specific JDK types shown when writing the review issue; the Platform generally assesses behavior.

| API family and earlier work | Required individual demonstration | Later AI-assisted reuse |
| --- | --- | --- |
| Strings, collections, generics and streams. Piscine List, Map, Set and Stream exercises. | In buy-02 or a capstone fixture, group records by owner, handle duplicates and empty input, then change the ordering. Explain list versus set and the reduction result. | Repeated mapping and display aggregates in commerce projects after review. |
| Object contracts, exceptions and resource lifetime. Piscine interfaces, inheritance, exceptions and file exercises. | In lets-play, map a missing resource and invalid input to distinct outcomes. In java-localserver close resources on early failure; explain lifetime and test cleanup. | Repeated DTOs and error response shapes. |
| Files, byte/text boundaries, time and parsing. Piscine FileManager, FileSearch, ParseDate, FormatDate and Regex exercises. | Read a file with Path/Files and an explicit charset; preserve binary bytes on upload. In 01blog test timestamp ordering and offset handling. Choose and explain the boundary of input validation. | Repeated file adapters and display formatting. |
| Networking and nonblocking NIO. Mandatory java-localserver. | Explain a ServerSocketChannel, SocketChannel, Selector, SelectionKey and ByteBuffer on the request path. While one client holds an incomplete request, serve another. Distinguish a zero-byte read from EOF. Preserve unread bytes and resume a partial write. Change one condition and rerun the check. | Additional route configuration and socket test fixtures after individual review. Each learner owns the event loop behavior. |
| Process management. Mandatory java-localserver CGI. | Launch the configured CGI with ProcessBuilder. Trace input, output, exit and cleanup. Demonstrate handling a failed child without losing the server. | Repeated CGI fixtures and setup. |
| Concurrency and data consistency. Compare the single-threaded selector with shared state in Spring requests. | In buy-02 or the capstone, exercise competing updates with a controlled fixture. Explain the invariant and demonstrate where it is enforced. Do not add threads to the single-threaded server. | Repeated test setup. The learner chooses the invariant and failure assertion. |
| SQL access and transaction semantics. Relational capstone. | Follow one request through Java persistence to PostgreSQL. Change a migration, identify a parameter binding, and demonstrate commit versus rollback. As a cohort Java SE check, use a small JDBC PreparedStatement in a fixture and close the resources. | Repeated mappings in assignments that permit generation. For 01blog use conceptual coaching only. MongoDB CRUD in lets-play does not establish relational competence. |

The [piscine exercise map](https://github.com/zone01athens/java-full-stack-starter/blob/main/PATH.md) locates prior practice. The [Java SE 17 API](https://docs.oracle.com/en/java/javase/17/docs/api/) defines the library contracts. Angular, Spring, MongoDB, Cypher and Jenkins are assessed as separate technologies.

## Assignment decisions

The official briefs and audit links appear below. The individual demonstrations and AI boundaries are cohort decisions. “Extension” applies to an additional product or toolchain; all core Java checks above apply to everyone.

| Project and official team size | Subject or audit evidence | Individual demonstration and reuse decision |
| --- | --- | --- |
| lets-play · 1 | Spring Boot, MongoDB, user/product ownership, public reads, JWT, admin-only user access and defined error responses. | Implement one persisted mutation. Show owner success, another user's refusal and invalid input. Scaffold repeated CRUD only after that evidence. |
| java-localserver · 2–3 | Java core libraries, one thread, readiness-driven I/O, HTTP requests and CGI. The audit traces the selection loop, return values and client removal. | Every member passes the NIO and process checks above. Rotate parser, transport and process responsibilities. Static pages and fixtures are good AI candidates. Complete the full official assignment for credit. |
| angul-it · 1 | Multi-stage CAPTCHA, Angular routing, validation, progress restored after refresh and protected results. | Implement a stage, refresh mid-flow and try direct access to results. Change a validation rule unaided. AI can draft styles; preserve accessible behavior. |
| buy-01 · 2–4 | User, product and media services; role/ownership checks and validated uploads. | Trace a seller's upload from Angular through media and product association. Demonstrate refusal of another seller's mutation and invalid media. Reuse forms and routine CRUD after the earlier reviews. Cross-service behavior needs fresh evidence. |
| mr-jenk · 1–2 | Pipeline, reports and deployment. Audit emphasizes observed operation. | Show a controlled test failure blocking promotion, then trace a staged rollback. AI can draft repeated Jenkins syntax; learner owns promotion conditions and readback. |
| safe-zone · 1–2 | Dockerized SonarQube integrated with CI. Audit also asks for explanations. | Explain one rule and threshold. Show a failed quality gate, fix the finding and rerun the same gate. Reuse Jenkins plumbing. |
| buy-02 · 2–4 | Extends buy-01 with cart, pay-on-delivery checkout, orders, analytics, filtering, Jenkins and SonarQube. | Own an order and its failure path. Check ownership, totals and what persists on failure. Dashboard scaffolding and repeated delivery steps can use AI. Payment gateway integration is additional scope. |
| nexus · 1–2 · platform extension | Versioned Maven and container artifacts, repository configuration and pipeline integration. | Inspect a versioned artifact in the common delivery review. To claim Nexus operation, publish two versions and resolve a pinned artifact from a clean client. Reuse the reviewed pipeline skeleton. |
| neo-4-flix · 1–2 · graph extension | Neo4j movie recommendations, Spring services, Angular and Docker. Audit asks about Cypher. | Confirm the expected mapping/graph library with the auditor: the rubric names Neo4j OGM and the Graph Algorithms Library. Change a recommendation on a known graph, predict the result and handle missing ratings. Reuse UI and CRUD. Graph modeling and Cypher require their own demonstration. |
| 01blog · 1 | Relational SQL, Spring, Angular, user content, reporting and moderation. PostgreSQL is the cohort choice. | Trace a post through UI, service and database. Test access and a moderation decision. Change a requirement unaided. Build the submitted code manually. The subject prohibits code generators (JHipster is its example). For this cohort, restrict AI to conceptual coaching on this assignment. |
| travel-plan · 4–6 · infrastructure extension | Admin dashboard, Ansible, multiple stores and replicated deployment. | Reuse the dashboard and delivery wiring. Own one Ansible change, demonstrate repeat application and failover, and explain which data belongs in each store. |
| lets-travel · 4–6 · product extension | Extends travel-plan with three roles, indexed search, recommendations, subscriptions and payments. | Trace a change through the stores. Check a cutoff boundary and a sandbox payment failure. Reuse reviewed infrastructure and UI. Search consistency, recommendation logic and payment behavior require new evidence. |

## Three individual checks carried forward from the piscine

Budget 30–40 minutes per check within existing project time. Use unfamiliar inputs and allow the JDK reference. For students who have finished the piscine, run these against the first matching specialization issue. The checks supplement existing Platform exams.

1. **Input and files.** Given a CLI transform, handle a malformed number, a missing file and UTF-8 input. Explain charset choice, exception handling and which resource the code owns.
2. **Collections and money.** Aggregate a small cart with duplicate and empty entries. Change the tie-break rule live. Choose an absence representation, then demonstrate an exact total using integer minor units or BigDecimal. Keep database pagination and aggregation in the database where appropriate.
3. **Time and validation.** Parse and format a date with a named formatter, compare a calendar period with elapsed time and distinguish a full regex match from a substring match. Change an input boundary and predict the result before running it.

Record the fixture, prediction, observed result and the learner's unaided change. In group projects record the reviewed diff and the member who demonstrated it. Recheck a missed criterion with a fresh variation. These are required individual cohort checks; no separate optional lab is needed.

## Source discrepancies that affect grading

- 01blog permits a relational SQL database; PostgreSQL is our choice. The brief explicitly prohibits code-generation tools. The cohort uses coaching only here.
- buy-01 mentions polyglot storage as an objective but lists MongoDB in its constraints. Use MongoDB for the official submission. Kafka is a suggestion in the subject.
- For team attribution use assignment group bounds from the Platform graph. Commentary inside the buy-01 and lets-travel competence maps describes solo work despite their group metadata.
- A deployment visible in Jenkins or a passing audit of a team artifact leaves individual understanding unverified. Use the fresh variation in the matrix as additional cohort evidence. Project skill weights carry no individual pass threshold.

## Planning at 15 hours per learner per week

Start with one 15-hour planning unit: 3 hours for API reading and hand-tracing, 8 for implementation and tests, 4 for pairing, individual variation and feedback. Repeat the unit as needed. For the NIO unit, the exit evidence is the two-client test and an individual explanation of partial I/O; finishing that unit does not complete java-localserver. Use actual first-week evidence to schedule later milestones. Team size follows the official assignment; identify common on-campus blocks before assigning partners. Do not infer a completion date from XP or skill weights.

## Sources and limits

On 27 November 2026 the subject and audit text for all 12 projects matched the Athens curriculum snapshot `4fa3767474a40955c7db5429fec0a13251f0e8fe` (whitespace-normalized comparison). We also reviewed the per-project competence maps and relation metadata for skill tags, prerequisites and team sizes. A tag describes curriculum intent; the individual review supplies evidence. Public upstream names and briefs can differ from Athens. Use the Athens assignment at submission time.

- lets-play · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/lets-play/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/lets-play/audit/README.md)
- java-localserver · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/java-localserver/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/java-localserver/audit/README.md)
- angul-it · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/angul-it/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/angul-it/audit/README.md)
- buy-01 · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/buy-01/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/buy-01/audit/README.md)
- mr-jenk · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/mr-jenk/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/mr-jenk/audit/README.md)
- safe-zone · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/safe-zone/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/safe-zone/audit/README.md)
- buy-02 · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/buy-02/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/buy-02/audit/README.md)
- nexus · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/nexus/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/nexus/audit/README.md)
- neo-4-flix · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/neo-4-flix/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/neo-4-flix/audit/README.md)
- 01blog · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/01blog/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/01blog/audit/README.md)
- travel-plan · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/travel-plan/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/travel-plan/audit/README.md)
- lets-travel · [Subject](https://platform.zone01.gr/api/content/root/01-edu_module/content/lets-travel/README.md) · [Audit](https://platform.zone01.gr/api/content/root/01-edu_module/content/lets-travel/audit/README.md)
