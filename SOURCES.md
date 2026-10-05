# Sources — Canadian Privacy Scan

A record of where this scan's information comes from. It has three parts:

1. **Monitored sources**: where each update looks for new developments.
2. **Cited in the current edition**: every source linked on the live page, rebuilt from `scan.json` by `python3 tools/sources.py`.
3. **Update log**: one row per update, recording what was checked and what changed.

Older editions' sources stay in the git history of this file.

## 1. Monitored sources

### Primary sources (cite these first)

| Source | What to check |
|---|---|
| [LEGISinfo](https://www.parl.ca/legisinfo) | Federal bill stages (C-36, C-34, C-22, new privacy, AI, cyber or online-safety bills) |
| [openparliament.ca](https://openparliament.ca) | Bill summaries and debate dates (backup when LEGISinfo won't load) |
| [Office of the Privacy Commissioner of Canada](https://www.priv.gc.ca) | News releases, reports of findings, guidance, advice to Parliament |
| [Commission d'accès à l'information du Québec](https://www.cai.gouv.qc.ca) | News, decisions, sanctions, guidance |
| [OIPC British Columbia](https://www.oipc.bc.ca) | Investigation reports, orders, guidance |
| [OIPC Alberta](https://oipc.ab.ca) | Investigation reports, orders, guidance |
| [IPC Ontario](https://www.ipc.on.ca) | Guidance, decisions (PHIPA, FIPPA/MFIPPA) |
| [Supreme Court of Canada](https://www.scc-csc.gc.ca) | Pending: *Facebook v. Privacy Commissioner* (No. 41538) |
| [CanLII](https://www.canlii.org) | Appellate privacy decisions, class action certification rulings |
| [ISED](https://ised-isde.canada.ca) | AI and privacy policy, consultations |
| [Treasury Board Secretariat](https://www.canada.ca/en/treasury-board-secretariat.html) | Privacy Act modernization |
| [Canada Gazette](https://gazette.gc.ca) | Regulations and coming-into-force orders |

### News (use to spot developments; cite only when no primary source exists)

| Source | Notes |
|---|---|
| [The Globe and Mail](https://www.theglobeandmail.com) | Canadian technology, politics and business coverage. Paywalled. |
| [The Washington Post](https://www.washingtonpost.com) | US technology coverage affecting Canadian privacy (cross-border platforms, AI companies). Paywalled. |

### Secondary analysis (used when no primary source is published)

Law firm bulletins (e.g., Fasken, Osler, Bennett Jones, McCarthy Tétrault, Blakes, Gowling WLG) and IAPP. Prefer the regulator's own document when it exists.

## 2. Cited in the current edition

<!-- cited:start -->
_Generated from `scan.json` (current to 2026-10-04). Do not edit by hand._

### Monthly brief

- **Federal privacy reform is back.**
  - [LEGISinfo: Bill C-36](https://www.parl.ca/legisinfo/en/bill/45-1/c-36)
  - [openparliament.ca](https://openparliament.ca/bills/45-1/C-36/)
- **Regulators are testing AI against existing law.**
  - [OPC on OpenAI](https://www.priv.gc.ca/en/opc-news/speeches-and-statements/2026/s-d_260506/)
  - [Clearview, 2026 BCCA 67](https://www.dww.com/articles/clearview-ai-breached-bc-privacy-law-appeal-court-holds)
- **Deletion and anonymization are being checked.**
  - [OPC Loblaw findings](https://www.priv.gc.ca/en/opc-news/news-and-announcements/2026/nr-c_260305/)
- **Children are the theme of 2026.**
  - [Bill C-34 backgrounder](https://www.canada.ca/en/canadian-heritage/news/2026/06/government-of-canada-introduces-legislation-to-combat-online-harms-particularly-those-impacting-children.html)
  - [OPC children's code](https://www.priv.gc.ca/en/about-the-opc/what-we-do/consultations/completed-consultations/consultation-children-code/report_children-code_2026/)
  - [Global sweep summary](https://www.carters.ca/?p=15717)

### Items

- **Quebec regulator proposes 74 reforms, including consent you set once in your browser** · QC · 2026-10-01 · last checked 2026-10-04
  - Citation: CAI, rapport quinquennal 2026, ss. 2.1.1 and 2.2; CAI news item, Oct. 1, 2026.
  - [CAI: consent (français)](https://www.cai.gouv.qc.ca/actualites/evolution-des-technologies-reflechir-au-role-du-consentement)
  - [CAI: five-year report (français)](https://www.cai.gouv.qc.ca/actualites/publication-du-rapport-quinquennal-2026-de-la-commission)
- **BC commissioner publishes identity theft guidance for organizations and individuals** · BC · 2026-08-31 · last checked 2026-10-04
  - Citation: OIPC BC news release, Aug. 31, 2026.
  - [OIPC BC news](https://oipc.bc.ca/documents/news-releases/3228)
- **Ontario updates its privacy impact assessment guide for public institutions** · ON · 2026-08-13 · last checked 2026-10-04
  - Citation: IPC Ontario, Planning for Success: Privacy Impact Assessment Guide (Aug. 2026).
  - [IPC Ontario guide](https://www.ipc.on.ca/en/resources/planning-success-privacy-impact-assessment-guide-ontarios-public-institutions)
- **Federal Privacy Act modernization: Commissioner backs Treasury Board proposals** · FED · 2026-08-06 · last checked 2026-10-04
  - Citation: OPC submission to Treasury Board Secretariat, Aug. 6, 2026.
  - [OPC news release](https://www.priv.gc.ca/en/opc-news/news-and-announcements/2026/nr-c_260806/)
- **AI transparency consultation closed September 23** · FED · 2026-07-23 · last checked 2026-10-04
  - Citation: ISED consultation, July 23 – Sept. 23, 2026.
  - [ISED announcement](https://www.canada.ca/en/innovation-science-economic-development/news/2026/07/government-of-canada-launches-public-consultation-on-ai-transparency.html)
- **Bill C-22: lawful access bill has passed the House and is in the Senate** · FED · 2026-06-18 · last checked 2026-10-04
  - Citation: Bill C-22, Lawful Access Act, 2026. Sponsor: Hon. Gary Anandasangaree, Minister of Public Safety. At second reading in the Senate as of June 18, 2026.
  - [OPC submission to SECU](https://www.priv.gc.ca/en/opc-actions-and-decisions/advice-to-parliament/2026/parl_260526/)
  - [openparliament.ca](https://openparliament.ca/bills/45-1/C-22/)
- **Bill C-36: a new federal private-sector privacy law is before Parliament** · FED · 2026-06-15 · last checked 2026-10-04
  - Citation: Bill C-36, 45th Parl., 1st Sess. Sponsor: Hon. Evan Solomon, Minister of Artificial Intelligence and Digital Innovation. First reading June 15, 2026.
  - [LEGISinfo: Bill C-36](https://www.parl.ca/legisinfo/en/bill/45-1/c-36)
  - [openparliament.ca summary](https://openparliament.ca/bills/45-1/C-36/)
  - [WeirFoulds analysis](https://www.weirfoulds.com/bill-c-36-and-the-future-of-canadas-federal-private-sector-privacy-law-what-has-changed-what-it-means-and-what-to-do-now)
- **Bill C-8: critical infrastructure cybersecurity law received Royal Assent** · FED · 2026-06-15 · last checked 2026-10-04
  - Citation: S.C. 2026, c. 9 (former Bill C-8).
  - [openparliament.ca](https://openparliament.ca/bills/45-1/C-8/)
- **Bill C-34: Safe Social Media Act would restrict accounts for under-16s and cover AI chatbots** · FED · 2026-06-10 · last checked 2026-10-04
  - Citation: Bill C-34, 45th Parl., 1st Sess. Introduced June 10, 2026 (Canadian Heritage).
  - [Government backgrounder](https://www.canada.ca/en/canadian-heritage/news/2026/06/government-of-canada-introduces-legislation-to-combat-online-harms-particularly-those-impacting-children.html)
  - [openparliament.ca](https://openparliament.ca/bills/45-1/C-34/)
- **Privacy class actions: courts keep screening out weak claims, but Quebec and BC remain open doors** · MULTI · 2026-06-04 · last checked 2026-10-04
  - Citation: See cases listed. Roundups: Bennett Jones (June 2026), McCarthy Tétrault (May 2026).
  - [McCarthy Tétrault roundup](https://www.mccarthy.ca/en/insights/publications/data-breach-class-actions-key-developments-and-emerging-risks-2026-privacy-breach-insights-part-2)
- **National AI strategy commits to a fundamental right to privacy in law** · FED · 2026-06-04 · last checked 2026-10-04
  - Citation: Launched June 4, 2026, by PM Carney and Minister Solomon.
  - [Gowling WLG summary](https://gowlingwlg.com/en/insights-resources/articles/2026/canada-launches-ai-for-all-national-artificial-intelligence-strategy)
- **Complaints to the federal Privacy Commissioner more than doubled** · FED · 2026-06-04 · last checked 2026-10-04
  - Citation: OPC Annual Report to Parliament 2025-2026, released June 4, 2026.
  - [OPC news release](https://www.priv.gc.ca/en/opc-news/news-and-announcements/2026/nr-c_260604/)
- **PowerSchool breach: commissioners fault school boards for weak vendor oversight** · MULTI · 2026-05-12 · last checked 2026-10-04
  - Citation: Ontario IPC and Alberta OIPC reports (Nov. 18, 2025); NL OIPC Report P-2026-001.
  - [NL OIPC release](https://www.gov.nl.ca/releases/2026/oipc/0512n01/)
  - [The Logic](https://thelogic.co/briefing/privacy-commissioners-castigate-school-boards-responses-to-powerschool-cyberbreach/)
- **OpenAI breached Canadian privacy law in building ChatGPT, four commissioners find** · MULTI · 2026-05-06 · last checked 2026-10-04
  - Citation: Joint investigation of OpenAI OpCo, LLC (OPC, CAI, OIPC BC, OIPC AB), May 6, 2026. Complaint opened April 4, 2023.
  - [Commissioner's statement](https://www.priv.gc.ca/en/opc-news/speeches-and-statements/2026/s-d_260506/)
  - [CAI (français)](https://www.cai.gouv.qc.ca/actualites/resultats-enquete-conjointe-sur-openai-chatgpt)
- **Children's privacy: global sweep finds most age checks easy to bypass; Canadian code in preparation** · MULTI · 2026-03-25 · last checked 2026-10-04
  - Citation: GPEN sweep results announced March 25, 2026; OPC, What We Heard report on the Children's Privacy Code consultation (2026).
  - [OPC consultation report](https://www.priv.gc.ca/en/about-the-opc/what-we-do/consultations/completed-consultations/consultation-children-code/report_children-code_2026/)
  - [Carters summary of the sweep](https://www.carters.ca/?p=15717)
- **Supreme Court has heard Facebook v. Privacy Commissioner; decision pending** · FED · 2026-03-19 · last checked 2026-10-04
  - Citation: Facebook, Inc. v. Privacy Commissioner of Canada, SCC No. 41538.
  - [SCC case docket](https://www.scc-csc.gc.ca/cases-dossiers/search-recherche/41538)
  - [Bennett Jones preview](https://www.bennettjones.com/Insights/Blogs/2026/03/Privacy-Goes-to-the-Top-Court)
- **Loblaw kept PC Optimum shopping histories after accounts were deleted** · FED · 2026-03-05 · last checked 2026-10-04
  - Citation: OPC, investigation of complaints regarding the PC Optimum program (news release March 5, 2026).
  - [OPC news release](https://www.priv.gc.ca/en/opc-news/news-and-announcements/2026/nr-c_260305/)
- **Clearview AI loses its BC appeal: scraping faces from the web broke privacy law** · BC · 2026-02-18 · last checked 2026-10-04
  - Citation: Clearview AI Inc. v. British Columbia (Information and Privacy Commissioner), 2026 BCCA 67 (Feb. 18, 2026). BC PIPA, SBC 2003, c. 63.
  - [Dentons/DWW summary](https://www.dww.com/articles/clearview-ai-breached-bc-privacy-law-appeal-court-holds)
  - [CTV News](https://www.ctvnews.ca/vancouver/article/clearview-ai-loses-bc-appeal-of-findings-over-facial-recognition-privacy-breaches/)
- **Ontario guidance on AI scribes in health care** · ON · Jan 2026 · last checked 2026-10-04
  - Citation: IPC Ontario, AI Scribes: Key Considerations for the Health Sector (January 2026), under PHIPA.
  - [Baker McKenzie analysis](https://www.bakermckenzie.com/en/insight/publications/2026/03/canada-ontario-ai-scribe-guidance-signals-emerging-regulatory-baseline)
  - [IPC Ontario](https://www.ipc.on.ca/)

_19 items, 30 unique source links._
<!-- cited:end -->

## 3. Update log

| Date | Checked | Added | Changed | Removed |
|---|---|---|---|---|
| 2026-10-04 | First edition. Federal bills, OPC, CAI, BC/AB/ON commissioners, SCC docket, law firm roundups | 19 items | — | — |
| 2026-10-05 | Bill C-36 penalty provisions (ss. 114, 145) | — | C-36 item and brief: highest fines are offence fines under s. 145 ($25M / 5% on indictment; $20M / 4% summary); $10M / 3% relabelled as the s. 114 administrative penalty cap | — |
