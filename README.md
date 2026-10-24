## Nikola Vukadin

Mechanical engineer. Industrial fluid systems, valve and flow control, and the technical writing that goes with them.

Serbia. Technical sales at EGAL Intech since October 2026.

---

### What I do

**Size and specify flow control equipment.** Valves, pumps, hydraulic and pneumatic circuits. I have surveyed and catalogued over 1,500 valves across a tyre manufacturing plant and specified equipment for process, oil and gas, and mining installations.

**Write technical content for engineers.** I audited over 200 technical articles for a European B2B distributor of industrial components, backed my recommendations with search analytics data, and wrote a selection guide on solenoid valve operating principles. I also publish [AI visibility audits](https://github.com/wule15/citation-case-studies) of industrial companies: what an AI crawler can read on their sites, and which suppliers four AI answer engines actually name.

**Run the commercial side of technical sales.** I issued EUR 300K to 500K of proposals over roughly two years, personally producing around 70 percent of them, and led a technical department of five to eight people.

**Build the tools when buying them does not fit.** Both code repositories below are mine, and both have test suites.

---

### Code

**[Flow-coef-calc](https://github.com/wule15/Flow-coef-calc)** - valve sizing to EN IEC 60534-2-1:2011. Liquid and gas flow coefficient, the choked flow check, the Reynolds number factor FR for viscous flow on both paths, a cited fluid property table, and material screening in both ASME and EN designations. Standard library only, 331 tests.

It is built around one idea: a sizing calculation returns a number, and the number cannot tell you the valve is choked, that the flow went laminar, or that Joule-Thomson cooling took the body below what its material is rated for. So it reports what it checked, and says plainly when it did not check something.

A [browser calculator](https://wule15.github.io/Flow-coef-calc/) ports the common liquid and gas cases to JavaScript, without the viscous correction, and is checked against the library.

**[Job-intelligence-agent](https://github.com/wule15/Job-intelligence-agent)** - a daily pipeline that reads company careers boards (Greenhouse, Lever, Ashby, SmartRecruiters, Workday, SuccessFactors) and other job sources, deduplicates, filters on eligibility, title, language, experience and degree rules, scores each listing against my CV variants and sends a capped Telegram digest. It keeps a send history and holds back jobs already sent. Python, no agent or scraping framework, 1267 tests.

One test file runs whole days through the real pipeline, from search to the Telegram message, with every network call faked and a temporary database. It runs once a day as a Google Cloud Run job, built from the included Dockerfile.

The README documents a bug that quietly discarded 86 percent of results for weeks, why it took so long to notice, and what changed as a result. That section is there on purpose.

---

### Background

BSc Mechanical Engineering, Energy and Process Engineering, University of Novi Sad. MSc Oil and Gas in progress.

ATEX certified. ePlan Fundamentals. FEA, Brno University of Technology.

Serbian native, English fluent, German intermediate.

---

### Get in touch

[Portfolio and case studies](https://cotton-booklet-950.notion.site/Nikola-Vukadin-Portfolio-3464d524ee72816b871cf66171ff89eb), [LinkedIn](https://www.linkedin.com/in/nikola-vukadin), or open an issue on any of the repositories above.
