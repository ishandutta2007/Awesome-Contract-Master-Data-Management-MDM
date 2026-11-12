# Awesome-Contract-Master-Data-Management-MDM

## Top Contract Master Data Management (MDM) Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Golden Record Creation, Entity Resolution & Cross-System Contract Data Consistency*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Contract Master Data Management (MDM)**. These tools help organizations create a single, trusted view of contract-related master data—counterparties, legal entities, suppliers, and pricing structures—across CRM, ERP, CLM, and procurement systems. They resolve duplicates, enforce data standards, and govern who can change critical fields like bank accounts or legal names.

**Examples** include Informatica MDM, SAP Master Data Governance, Semarchy xDM, Profisee, Reltio, Stibo Systems, Tibco EBX, Ataccama ONE, Icertis, and Pimcore (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted MDM, open-source entity resolution, and community-driven data governance—ideal for organizations seeking data sovereignty and transparent matching logic over opaque enterprise licensing. Note that the open-source MDM landscape is genuinely thin in 2026: Talend Open Studio for MDM was retired in January 2024, and Pimcore's Community Edition now has a €5M revenue threshold [citation:2].

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Informatica MDM](https://www.informatica.com/)** | Enterprise master data management with multi-domain support, match-and-merge, and data stewardship workflows. Widely deployed for customer and supplier master data across large organizations. | Quote-only (enterprise contract; typically six-figure annual) | No free tier; demo via sales |
| **[SAP Master Data Governance](https://www.sap.com/)** | MDM embedded within SAP S/4HANA and ECC. Central governance for supplier, customer, and material master data with approval workflows and consolidation. Tight integration with SAP ERP. | Quote-only (bundled with SAP licensing; separate MDG license required) | No free tier; demo via SAP sales |
| **[Semarchy xDM](https://www.semarchy.com/)** | Unified MDM platform with a single data model, match-and-merge, and workflow-driven stewardship. Positioned for mid-market and enterprise deployments. | Quote-only (subscription-based) | No free tier; demo via sales |
| **[Profisee](https://profisee.com/)** | MDM platform built on Microsoft Azure. Fast deployment (claims go-live in 8–12 weeks), native Azure integration, and stewardship workflows. | Quote-only (subscription-based) | No free tier; demo via sales |
| **[Reltio](https://www.reltio.com/)** | Cloud-native MDM with real-time entity resolution, graph-based relationship modeling, and multidomain support. Positioned for customer 360 and life sciences. | Quote-only (enterprise subscription) | No free tier; demo via sales |
| **[Stibo Systems](https://www.stibosystems.com/)** | Multidomain MDM with strong product information management (PIM) heritage. Used heavily in retail and manufacturing for product and supplier master data. | Quote-only (enterprise contract) | No free tier; demo via sales |
| **[Tibco EBX](https://www.tibco.com/)** | Unified MDM and data governance platform. Model-driven approach with strong workflow and stewardship capabilities. | Quote-only (enterprise contract) | No free tier; demo via sales |
| **[Ataccama ONE](https://www.ataccama.com/)** | Data quality and MDM platform combining profiling, cleansing, matching, and stewardship in a single environment. | Quote-only (subscription-based) | No free tier; demo via sales |
| **[Icertis](https://www.icertis.com/)** | Contract intelligence platform with Global Master Data Management capabilities for counterparty and contract metadata. Creates a golden record for legal entities referenced across contracts. | Quote-only (enterprise contract) | No free tier; demo via sales |
| **[Pimcore](https://pimcore.com/)** | Open-core data and experience management platform covering PIM, MDM, DAM, and DXP. **Community Edition is free only for organizations with ≤€5M annual turnover**; above that a commercial license is required (Professional at $9,900/year, Enterprise at $29,900/year) [citation:2][citation:7]. | Professional: $9,900/year; Enterprise: $29,900/year; Community: free under €5M revenue [citation:7] | Community Edition free only under €5M revenue; no trial mentioned for paid tiers |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[AtroCore / AtroPIM](https://github.com/atrocore/atrocore)** | [![Stars](https://img.shields.io/github/stars/atrocore/atrocore?style=social&color=white)](https://github.com/atrocore/atrocore/stargazers) | **The one genuinely open-source MDM/PIM candidate left in 2026** [citation:2]. GPLv3, PHP-based, runs on PostgreSQL, MySQL, or MariaDB. The core and a set of modules are free; ERP and e-commerce integrations are paid premium modules. Includes match-and-merge, data quality rules, and stewardship workflows. Premium modules €20–90/month each (SaaS) or €500–2,250 one-time (on-premises); ERP integrations from €1,900 [citation:7]. |
| **[Yugandhar Open MDM Hub](https://github.com/yugandharproject/yugandhar-open-mdmhub)** | [![Stars](https://img.shields.io/github/stars/yugandharproject/yugandhar-open-mdmhub?style=social&color=white)](https://github.com/yugandharproject/yugandhar-open-mdmhub/stargazers) | Open-source MDM hub for customer data integration (CDI). Apache 2.0. Built on Spring Boot, Hibernate, and JBoss. Includes 450+ prebuilt REST/MQ services, match-and-merge framework, audit logging, and a preconfigured data model for Person and Organization master data [citation:1]. Last release appears to be from 2018; treat as a reference architecture rather than actively maintained software. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[OpenMetadata](https://github.com/open-metadata/OpenMetadata)** | [![Stars](https://img.shields.io/github/stars/open-metadata/OpenMetadata?style=social&color=white)](https://github.com/open-metadata/OpenMetadata/stargazers) | **Important distinction**: OpenMetadata is a **data catalog**, not an MDM system. It tells you which tables exist and what columns mean; it does not decide which of three supplier addresses is correct [citation:2]. Useful as a complementary layer for discovering where contract-related data lives across databases. |
| **[DataHub](https://github.com/datahub-project/datahub)** | [![Stars](https://img.shields.io/github/stars/datahub-project/datahub?style=social&color=white)](https://github.com/datahub-project/datahub/stargazers) | Another metadata catalog, not MDM. Provides lineage and search across data assets. Same caveat applies: catalogs describe data; MDM decides the golden record [citation:2]. |
| **[Shillinq](https://github.com/ConductionNL/shillinq)** | [![Stars](https://img.shields.io/github/stars/ConductionNL/shillinq?style=social&color=white)](https://github.com/ConductionNL/shillinq/stargazers) | Nextcloud-based business administration suite with **contract repository, supplier management, and PO revision tracking**. Not a full MDM engine, but includes supplier qualification and approval chains that touch master data governance . EUPL-1.2. |

**Frameworks for building custom systems**: The open-source MDM landscape is genuinely sparse. **AtroCore** is the only actively maintained, GPL-licensed MDM/PIM option with real match-and-merge and stewardship capabilities [citation:2]. For customer master data specifically, **Yugandhar** provides a reference architecture but is not actively maintained. Organizations needing production-grade MDM with open-source licensing should budget for significant engineering effort to extend AtroCore or build custom matching logic on top of a data platform like PostgreSQL + Great Expectations.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- MDM platforms govern critical master data (supplier bank accounts, legal entity names, pricing structures); enforce strict approval workflows, audit trails, and segregation of duties. A wrong golden record propagates everywhere.
- **The open-source MDM landscape is thinner than it appears.** Talend Open Studio for MDM was retired in January 2024 and receives no security patches [citation:2]. Pimcore's Community Edition now has a €5M revenue threshold—most organizations shopping for MDM exceed this [citation:2][citation:7]. AtroCore is the one real GPL candidate, but its ERP integrations are paid modules [citation:2]. Data catalogs (OpenMetadata, DataHub) are frequently mistaken for MDM in search results; they solve a different problem [citation:2].

---

**Made for data governance teams, MDM architects, procurement data stewards, and developers building master data infrastructure.**  
Let's make contract master data management more open, transparent, and governable.
