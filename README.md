# Java specialization | Zone01 Athens

Build one portfolio application that an engineer can clone, test and review. Target Java, Spring Boot, Angular and PostgreSQL. The piscine has its [own repository](https://github.com/zone01athens/java-full-stack-starter) and schedule. Use the [specialization board](https://github.com/orgs/zone01athens/projects/9) for project decisions.

## Project selection

Recommended cohort scope: complete the two foundations and one individual capstone. Reuse the capstone for a small delivery lab. The other assignments are options, subject to Platform prerequisites. The table uses Athens assignment names.

| Assignment | Decision | What to build or assess |
| --- | --- | --- |
| lets-play | Core | Implement the Spring Boot API, persistence and role checks. Demonstrate a denied operation and a passing integration test. The official brief uses MongoDB. |
| java-localserver | Elective | HTTP parsing, nonblocking I/O and CGI are useful for systems roles. Defer the custom server for this application track. |
| angul-it | Core | Implement routing, validated forms and state through a multi-stage CAPTCHA. Test a failed validation and restoration of progress. AI can draft styling. |
| buy-01 | Optional commerce route | Implement a seller-to-catalog flow across Spring services and Angular. Use this as the base if pursuing buy-02 for credit. |
| mr-jenk | Assisted delivery lab | Apply build, test and deploy stages to the capstone. AI can draft Jenkins configuration. Break a test and demonstrate that promotion stops. |
| safe-zone | Assisted quality lab | Add a SonarQube gate. Students triage a real finding, fix it and show the before/after report. |
| buy-02 | Optional commerce route | Extend buy-01 with orders and checkout. Own transaction boundaries, authorization and failure tests. AI can draft dashboard scaffolding. |
| nexus | Defer | Maven and Docker artifact hosting is valuable for platform engineering. For this cohort, inspect one versioned artifact in the delivery lab. |
| neo-4-flix | Elective | Choose for graph-heavy roles. Model a recommendation and explain its Cypher query and data tradeoffs. |
| 01blog | Core capstone | Build the individual Spring–Angular application with PostgreSQL. Own schema migrations, role checks, moderation and end-to-end tests. |
| travel-plan | Defer | The travel dashboard repeats full-stack and delivery skills and adds Ansible and two databases. Select for an infrastructure-focused route. |
| lets-travel | Defer | Extends travel-plan with recommendations, subscriptions and payments. Requires the travel foundation and adds a second product domain. |

## Internal milestones and Platform credit

For the internal fast track, complete lets-play, angul-it, then the 01blog capstone with the delivery lab. Review code and evidence on GitHub. Skipping commerce projects affects official eligibility for 01blog.

For official 01blog credit, the Athens dependency graph is **piscine-java → lets-play → angul-it → buy-01 → mr-jenk → safe-zone → buy-02 → 01blog**. Complete each required assignment and audit, or obtain an approved Platform route change. A reduced lab alone does not satisfy an official project. The alternate travel route continues from buy-02 through nexus, neo-4-flix, travel-plan and lets-travel. java-localserver branches directly from piscine-java.

## Assessment and AI use

Each developer must explain a database migration, trace an Angular request through Spring to PostgreSQL, diagnose a failed test and implement a small change during review. AI may draft repetitive components, sample data, styling and pipeline boilerplate. The author reviews generated code, tests it and identifies the assisted portions in the PR. Apply the Platform's rules to every assessed submission.

## Market evidence

Selection reviewed 27 November 2026 against employer postings and the Athens project briefs. This is a targeted sample for an application-development track. It does not measure vacancy share.

- **Qualco, associate, Athens.** Spring Boot and enterprise application work support the backend foundation. JPA/Hibernate, Docker and CI/CD are additional skills. [Role](https://apply.workable.com/qualcogroup/j/E52F5B3019)
- **European Dynamics, Greece/remote.** Java, SQL and JavaScript/Angular support a single database-backed full-stack capstone. [Role](https://apply.workable.com/european-dynamics/j/151C739477)
- **PLANET, 1+ years.** Spring Boot, REST, Git, Maven and Docker support a short delivery lab. Jenkins is useful in this stack. [Role](https://apply.workable.com/planet-sa-1/j/601D56BBE0/apply)
- **QnR, senior comparator.** PostgreSQL, migrations and JPA show what the database skill develops into. Senior responsibilities are outside the entry assessment. [Role](https://apply.workable.com/qnr-1/j/D342CB5F5C)

[Restricted Educational License](LICENSE)
