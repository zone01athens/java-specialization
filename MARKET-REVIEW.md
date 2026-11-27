# Java specialization and the hiring market

Research snapshot, 27 November 2026. Keep Java, Spring, relational SQL, one frontend framework and delivery in the common track. Move SQL and independent debugging earlier. Assess the ability to change existing software as well as building a new application.

## Sample and interpretation

Ten distinct early-career role descriptions from ten employers: five in Greece and five in four other EU countries. Selection admitted junior, associate, graduate or explicit 1+ year roles with Java among the working languages. Two additional Greek descriptions illustrate a different seniority or specialization. Employer listings and employer-authored PDFs were read directly. Workable publication state was checked through its public job detail endpoint. A reachable PDF establishes the published role profile; current recruiting status for these PDFs was not verified. One employer contributes both a junior and a comparator role. Locations in a single posting count once.

Searches targeted Java, junior and enterprise web development, sometimes including Spring or SQL. The sample is deliberately relevant to this course, so mention counts cannot estimate market share or rank languages. Employer size was not consistently verified; the sample does not establish SME-specific prevalence. Hybrid openings abroad do not establish remote eligibility from Greece.

## Employer evidence

| Role and geography | Expected skills or work | Preferred skills, eligibility or limits |
| --- | --- | --- |
| European Dynamics, junior Java programmer, Athens or remote | Java development and SQL/database experience; degree listed. | Spring, Git and Maven desirable. Published 2 Nov 2026. [Employer](https://apply.workable.com/european-dynamics/j/736464CD1B) |
| Qualco, associate full stack, Athens | Java/OOP, Spring basics, SQL, REST/JSON, frontend basics, Git/builds, debugging, Greek and English. | Up to three years; React named. JPA, Docker/cloud and CI/CD listed as desirable. Published 10 Nov 2026. [Employer](https://apply.workable.com/qualcogroup/j/E52F5B3019) |
| PLANET, Java microservices developer, Athens hybrid | One or more years; Spring Boot, REST, Git, Maven, Docker, JPA, Linux. Work includes testing, debugging and releases. | React, Kubernetes/Helm and Jenkins are pluses. Published 12 Jun 2026. [Employer](https://apply.workable.com/planet-sa-1/j/601D56BBE0) |
| CloudOn, junior software developer, Athens | Java or Python backend work, unit and integration tests, Git, CI/CD basics, REST, SQL or NoSQL, troubleshooting via logs, review feedback. | Cloud or containers preferred. Equivalent technical education plus demonstrable experience accepted. Up to three days remote. [Employer](https://my.cloudon.gr/project/apply.php?job=5&lang=en) |
| ICAP CRIF, junior software developer, Greece | Java or C#, Spring Boot or .NET Core, relational databases, English B2 and team collaboration. | Angular, React or TypeScript, Git and Jira are assets. Historical employer PDF hosted by NTUA. [Role](https://career-net.ntua.gr/wp-content/uploads/2025/07/ICAP-CRIF-Junior-Software-Developer-Job-Ad.pdf) |
| EPAM, junior Java developer, Poland hybrid | One or more years in Java; JUnit, Mockito and SQL; English with clients. Full lifecycle includes support. | Location specified in Poland. [Employer](https://careers.epam.com/en/vacancy/junior-java-developer-blt13d7l9ysad6ry7dx_en) |
| 2e Systems, junior Java developer, Zagreb hybrid | Employer seeks experience in some or all of Java/OOP, data structures, relational SQL, Unix/networking, version control and specifications. Deployment support and diagnosis are job duties. | Spring/JPA, APIs, messaging and Maven appear as beneficial. Historical employer PDF. [Role](https://www.2e-systems.com/uploads/2025-08/8b66a3ddd99c55d70410ac5b40a716fd.pdf) |
| AEB, junior software developer, near Prague | First OOP experience, ideally Java; English; maintaining and extending an existing product. Java and SQL/NoSQL appear in the work environment. | German or Czech desirable. Role is based near Prague. [Employer PDF](https://www.aeb.com/media/docs/en/job-ads/junior-software-developer-prag.pdf) |
| Diebold Nixdorf, junior Java software engineer, Pilsen | Basic Java and SQL, XML/HTML, English and teamwork; contributes to product builds and configuration. | Version control and bug tracking desirable. [Employer PDF](https://www.dieboldnixdorf.com/en-us/-/media/diebold/files/czech-republish-openings/junior_java_ps) |
| ALTEN, graduate V.I.E Java backend engineer, Germany | Java, Spring Boot, backend experience, German and English; maintaining existing features and assisting deployments. | Kubernetes desirable; programme imposes age, degree and citizenship eligibility. [Employer PDF](https://www.alten-germany.de/en/jobs/744000159796539-v-i-e-java-backend-engineer-all-gender/pdf) |

**Comparators excluded from the ten.** European Dynamics explicitly lists JavaScript and/or Angular alongside SQL in an Athens/Crete/remote Java role without a junior label. QnR's senior role requests modernization, SQL/migrations, integration, tests and review of AI-generated work, with 5+ years of production experience. Use these to design a direction of progression. [European Dynamics](https://apply.workable.com/european-dynamics/j/151C739477) · [QnR](https://apply.workable.com/qnr-1/j/D342CB5F5C)

## Independent evidence

- Randstad Greece surveyed 127 technology companies within its 2026 HR Trends study (fieldwork October 2025–March 2026). 66% planned headcount growth. Teamwork was identified by 54% among future skills; 72% reported supporting AI and planning wider adoption. These are employer intentions across technology roles. [Sector report](https://www.randstad.gr/h-randstad/deltia-typou/deltia-typoy/ereyna-hr-trends-technology-apo-ti-randstad-oi-taseis-ston/)
- Eurostat reports 10.45 million EU ICT specialists in employment in 2025, or 5.0% of employment, versus 2.5% in Greece. In a different series, 57.5% of EU enterprises that attempted ICT recruitment in 2023 encountered difficulty. Neither series identifies junior Java vacancies. [Employment](https://ec.europa.eu/eurostat/en/web/products-eurostat-news/w/ddn-20260527-2) · [Recruitment denominator](https://ec.europa.eu/eurostat/statistics-explained/index.php?title=ICT_specialists_-_statistics_on_hard-to-fill_vacancies_in_enterprises)
- Stack Overflow's 2025 global survey placed PostgreSQL first on its desired and admired database measures. Its respondents were recruited primarily through Stack Overflow channels. This supports PostgreSQL as a practical teaching choice; local postings give the hiring evidence for relational SQL generally. [Technology](https://survey.stackoverflow.co/2025/technology) · [Methodology](https://survey.stackoverflow.co/2025/methodology)

## Curriculum decisions supported by the review

| Projects | Teaching decision | Proposed individual evidence |
| --- | --- | --- |
| lets-play and 01blog | Keep Spring and HTTP ownership. Introduce SQL alongside the first project in a separate fixture; preserve MongoDB for the official lets-play submission. Teach relational modeling, joins, constraints, migrations, JPA-generated SQL and rollback. | Answer a business question with a JOIN; then trace a wrong API result from request to stored value. |
| java-localserver | Keep mandatory. Market evidence supports networking, Linux and diagnosis; the direct reason for selector, buffer and CGI depth is the Java curriculum and audit. | Diagnose a stalled client while another completes. Explain partial I/O and cleanup. |
| angul-it | Keep Angular and TypeScript as the implementation stack. Teach transferable browser skills: HTTP, forms, state, accessibility, errors and routing. React appears alongside or instead of Angular in employer descriptions. | Restore progress after refresh; handle a rejected API request and test the UI state. |
| buy-01 and buy-02 | Spend mentoring on boundaries, ownership, accurate totals, transactions and failure cases. Make one change against an existing service. | Reproduce a defect, write a failing regression, fix it and describe the trade-off in an English PR. |
| mr-jenk and safe-zone | Keep Git, builds, automated tests, Docker, logs and CI diagnosis. Jenkins and SonarQube are implementations in this course. | From a clean clone, build and run the service; diagnose a failing pipeline and demonstrate recovery. |
| nexus, neo-4-flix, travel-plan and lets-travel | Retain outside the common product route. Current sample provides insufficient evidence to spend common hours on registry administration, graph algorithms, Ansible, multi-store search or payment integration. | Offer as role-specific depth when a target employer or project requires it. |

The most useful portfolio addition is one small maintenance PR per learner: reproduce an unfamiliar defect, add a regression test, explain the cause, and review a teammate's change. Use this inside an existing milestone and preserve the 15-hour weekly budget. Degree, language and experience filters remain relevant to matching; a portfolio demonstrates ability but cannot guarantee eligibility.

## PostgreSQL and workshops

PostgreSQL is the shared relational database for the cohort. Introduce it during lets-play in a separate fixture and use it for the 01blog application. Keep MongoDB in official submissions that require it. Schedule workshops inside the existing 15-hour week. Allocate 90 minutes to each workshop and use the learner's next project PR for individual evidence.

| When | Hands-on workshop | Individual follow-through |
| --- | --- | --- |
| Alongside lets-play | PostgreSQL: create an owner/product schema, add foreign keys, break a constraint and query owners with zero products. | Write and explain a LEFT JOIN against a new fixture. |
| During java-localserver | Java networking: inspect a fragmented request and follow the buffer through the selector loop. | Reproduce and explain an incomplete read in the team's implementation. |
| Before buy-02 checkout | PostgreSQL transactions: use two sessions to attempt the last unit of stock. Observe commit, failure and rollback. | Write an integration test that proves stock cannot become negative. |
| During mr-jenk and safe-zone | Docker, Linux logs and CI: diagnose a failing service and restore a passing build. | Submit a regression test and an English PR describing the cause and how to verify the fix. |
| During 01blog | PostgreSQL and JPA: inspect emitted SQL, spot redundant queries and compare query plans before and after one index. | Explain a measured change using representative data and review the migration in the capstone. |
