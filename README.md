# Java specialization | Zone01 Athens

Build one portfolio application that an engineer can clone, test and review. Target Java, Spring Boot, Angular and PostgreSQL. The piscine has its [own repository](https://github.com/zone01athens/java-full-stack-starter) and schedule. Use the [specialization board](https://github.com/orgs/zone01athens/projects/9) for project decisions.

## Weekly work and workshops

Plan for **15 hours per learner per week**, including workshops and individual review. Collect recurring campus availability before assigning teams. Track each milestone on the specialization board and link its issue to the implementation, tests and individual demonstration. The allocation is a planning budget; calendar dates depend on team availability and progress.

Five proposed 90-minute workshops follow the projects:

| When | Workshop | Evidence in the next PR or review |
| --- | --- | --- |
| Alongside lets-play | PostgreSQL schema, constraints and joins | Explain a LEFT JOIN that includes owners with zero products. Keep this fixture separate from the official MongoDB submission. |
| During java-localserver | Java NIO and fragmented requests | Trace a partial read while a second client completes a request. |
| Before buy-02 checkout | PostgreSQL transactions | Use two sessions competing for the last unit and test the stock invariant. |
| During mr-jenk and safe-zone | Docker, Linux logs and CI debugging | Reproduce a failure, add a regression test and explain the fix in an English PR. |
| During 01blog | JPA, PostgreSQL query plans and indexes | Inspect the SQL and measure the effect of one index using representative data. |

[Workshop exercises](MARKET-REVIEW.md#postgresql-and-workshops) · [Weekly planning](SKILL-MAP.md#planning-at-15-hours-per-learner-per-week)

## Project selection

Study four projects in depth: lets-play, java-localserver, angul-it and 01blog. Focus on the new skills in buy-01, mr-jenk, safe-zone and buy-02. These four are prerequisites for official 01blog credit. The remaining four projects are outside the common track. See the [skill map](SKILL-MAP.md) for individual checks and permitted AI assistance.

| Assignment | Decision | What to build or assess |
| --- | --- | --- |
| lets-play | Core | Implement the Spring Boot API, persistence and role checks. Demonstrate a denied operation and a passing integration test. The official brief uses MongoDB. |
| java-localserver | Core Java systems project | Implement the event loop, socket I/O, HTTP framing and CGI lifecycle. Each team member passes an individual transfer check. |
| angul-it | Core | Implement routing, validated forms and state through a multi-stage CAPTCHA. Test a failed validation and restoration of progress. AI can draft styling. |
| buy-01 | Selective depth | Implement a seller-to-catalog flow across Spring services and Angular. Use this as the base if pursuing buy-02 for credit. |
| mr-jenk | Selective depth | Apply build, test and deploy stages to the capstone. AI can draft Jenkins configuration. Break a test and demonstrate that promotion stops. |
| safe-zone | Selective depth | Add a SonarQube gate. Students triage a real finding, fix it and show the before/after report. |
| buy-02 | Selective depth | Extend buy-01 with orders and checkout. Own transaction boundaries, authorization and failure tests. AI can draft dashboard scaffolding. |
| nexus | Outside common track | Maven and Docker artifact hosting is valuable for platform engineering. For this cohort, inspect one versioned artifact in the delivery lab. |
| neo-4-flix | Outside common track | Choose for graph-heavy roles. Model a recommendation and explain its Cypher query and data tradeoffs. |
| 01blog | Core capstone | Build the individual Spring–Angular application with PostgreSQL. Own schema migrations, role checks, moderation and end-to-end tests. |
| travel-plan | Outside common track | The travel dashboard repeats full-stack and delivery skills and adds Ansible and two databases. Select for an infrastructure-focused route. |
| lets-travel | Outside common track | Extends travel-plan with recommendations, subscriptions and payments. Requires the travel foundation and adds a second product domain. |

## Internal milestones and Platform credit

For the internal fast track, complete lets-play, java-localserver and angul-it before the 01blog capstone with the delivery lab. Schedule java-localserver after the piscine. Review code and evidence on GitHub. Skipping commerce projects affects official eligibility for 01blog.

For official 01blog credit, the Athens dependency graph is **piscine-java → lets-play → angul-it → buy-01 → mr-jenk → safe-zone → buy-02 → 01blog**. Complete each required assignment and audit, or obtain an approved Platform route change. A reduced lab alone does not satisfy an official project. The alternate travel route continues from buy-02 through nexus, neo-4-flix, travel-plan and lets-travel. java-localserver branches directly from piscine-java. This cohort requires the branch for its internal track.

## Assessment and AI use

Each developer must explain a database migration, trace an Angular request through Spring to PostgreSQL, diagnose a failed test and implement a small change during review. Where the assignment permits it, AI may draft repetitive components, sample data, styling and pipeline boilerplate after the learner demonstrates the underlying skill. For 01blog the subject prohibits code generators. The cohort uses conceptual coaching only. The author reviews generated code, tests it and identifies the assisted portions in the PR. Apply the Platform's rules to every assessed submission.

### Required skills and permitted AI reuse

Use the [audit-backed skill map](SKILL-MAP.md) to scope issues and assign individual reviews. Record the earlier demonstration before authorizing AI to scaffold repeated work. A technology with no demonstrated overlap has its own assessment or remains explicitly outside the route.

## Market evidence

The November 2026 review examined ten early-career roles in Greece and four other EU countries, plus two Greek comparator roles. Based on this sample, introduce relational SQL early, teach one frontend stack in depth, and require each learner to diagnose an unfamiliar defect, write a regression test and explain the change in review. The full report distinguishes required skills from employer preferences and documents the sample limits. [Employer evidence and surveys](MARKET-REVIEW.md)

[Restricted Educational License](LICENSE)
