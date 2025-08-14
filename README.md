# Agile Control Map (ACM)

> Map relevant IT frameworks (ITIL, COBIT, CIS Controls, ISO/IEC 27001/27002) to phases of agile solution development (SAFe) so teams can move fast and not break things.

![Status](https://img.shields.io/badge/status-research%20artifact-informational)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
![SAFe](https://img.shields.io/badge/framework-SAFe%205.x-2ea44f)
![Standards](https://img.shields.io/badge/refs-ITIL%204%20%7C%20COBIT%202019%20%7C%20ISO%2FIEC%2027001%2F27002%20%7C%20CIS%20Controls%20v8.1-8a2be2)

<details>
<summary><strong>Table of contents</strong></summary>

- [Overview](#overview)
- [Why this exists](#why-this-exists)
- [What the artifact does](#what-the-artifact-does)
- [Background &amp; scope](#background--scope)
- [Research questions](#research-questions)
- [Methodology](#methodology)
- [Getting started](#getting-started)
- [Usage](#usage)
- [Examples](#examples)
- [Data &amp; schema](#data--schema)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [Cite this work](#cite-this-work)
- [Acknowledgments](#acknowledgments)
- [License](#license)
- [Contact](#contact)
- [Disclaimer](#disclaimer)
</details>

---

## Overview

**Agile Control Map (ACM)** is a research artifact from a master’s thesis that helps agile teams using SAFe identify which IT governance, service management, and security controls to consider in each phase of solution development. It bridges the *Agile Universe* and the *Controlled Universe*, making non-functional and compliance requirements visible early enough to be planned, implemented, and validated.

**Project context:** Master’s thesis “Move Fast and Don’t Break Things — Mapping Relevant IT Frameworks (ITIL, COBIT, CIS Controls, ISO/IEC 27001/27002) to Phases of Agile Solution Development (SAFe)” by **Gerhard Schreihans**. Advisor: **Edgar Weippl**. Assistance: **Alexander Schatten**, **Philipp Reisinger**.

## Why this exists

Teams often overlook framework-driven requirements such as backups or segregation of duties because they do not add immediate user-facing functionality and therefore rarely become stories. The result can be security and quality gaps, especially across non-functional requirements. ACM surfaces these requirements at the right time in SAFe, so they can be sized and scheduled like any other work.

## What the artifact does

- Maps SAFe phases and activities to relevant practices and controls from **ITIL 4**, **COBIT 2019**, **ISO/IEC 27001:2022 & 27002:2022**, and **CIS Controls v8.1**.
- Highlights candidate inputs for **enabler** and **user stories** derived from those controls.
- Supports evaluation of the mapping via expert feedback (**ex-ante** interviews and **ex-post** survey).

## Background & scope

**Problem space:** Larger, regulated organizations want the speed of agile while maintaining robust Internal Control Systems; regulators require resilient governance and controls. ACM addresses the friction between value creation (agile) and risk reduction (governance).

**In-scope frameworks:** SAFe 5.x as process backbone with mappings to ITIL 4, COBIT 2019, ISO/IEC 27001/27002, and CIS Controls v8.1.

**Scope statement:** ACM does not invent a new framework; it uses existing ones to guide when specific controls and process steps should be considered.

## Research questions

- **RQ1.1–RQ1.4:** Which COBIT, ITIL, ISO/IEC 27001/27002, and CIS Controls should be considered in which SAFe phase when implementing new features?  
- **RQ2:** Which of those practices and controls can serve as inputs for enabler or user stories?  
- **RQ3:** How well does the resulting artifact map SAFe phases to the relevant practices and controls, as evaluated ex-ante and ex-post with subject-matter experts?

## Methodology

- **Systematic Literature Review** based on Kitchenham guidelines to collect and assess evidence on combining agile methods with IT frameworks.
- **Design Science approach (Hevner):** artifact design, ex-ante validation via expert interviews, and ex-post naturalistic evaluation via a broader expert survey. The artifact is considered acceptable if a majority evaluates it positively.

## Getting started

1. Add this repository to your workspace.  
2. Install any required dependencies for your chosen language or runtime using your standard package manager.  
3. Optionally set up a container or virtual environment.  
4. Configure the data files if you want to customize the mapping (see **Data & schema**).  
5. Build the outputs you need (e.g., CSV or Markdown exports) using your project’s standard process.

## Usage

- Explore which controls are relevant for a given SAFe phase or activity.  
- Derive enabler and user stories from mapped controls and include them in planning and refinement.  
- Share exports with teams for PI planning, governance reviews, or audits.  
- Capture organizational adaptations and rationales alongside the mapping.

## Examples

**Mapping table template** (fill with your concrete mappings; do not copy proprietary control texts):

| SAFe Phase or Activity | Framework            | Reference (ID or Name)            | Why here                                              | Story seed                                                    |
| --- | --- | --- | --- | --- |
| PHASE | ISO/IEC 27001:2022 | A.5.3 Segregation of duties | Role model and access design must start early | Design RBAC with SoD constraints; add tests. |
| PHASE | CIS Controls v8.1 | 11.2 Automated Backups | Plan, implement, and regularly test backup and restore | Automate backups; verify restore regularly. |
| PHASE | COBIT 2019 | APOxx or DSSxx | Governance or operations touchpoints | Define measurement and monitoring for CAPABILITY. |
| PHASE | ITIL 4 | PRACTICE_NAME | Service management integration | Update CMDB and change policy for SERVICE. |

**Story hint template (plain text):**

As a ROLE, I need CONTROL_REQUIREMENT during PHASE, so that RISK is reduced or COMPLIANCE is met and OUTCOME is achieved.
Acceptance: OBJECTIVE, TESTABLE CRITERIA.


## Data & schema

The mapping is maintained as a structured dataset that lists SAFe phases or activities alongside references to control identifiers and titles from the supported frameworks.

- The dataset should only contain identifiers, titles, and public metadata. **Do not include verbatim content from proprietary standards.**
- A simple schema (for example, JSON Schema or YAML schema) is recommended to ensure referential integrity and consistent taxonomy across files and exports.
- Typical exports include a human-readable Markdown table and a flat CSV for analysis in BI tools.

## Roadmap

- [ ] Publish version 1.0 mapping datasets (CSV, JSON, Markdown)  
- [ ] Add a simple query interface or command-line helper  
- [ ] Provide examples in notebooks or dashboards for exploration  
- [ ] Release an anonymized evaluation summary  
- [ ] Add importers for custom SAFe taxonomies  
- [ ] Integrate lint rules for story seeds and mapping consistency

## Contributing

Contributions are welcome.

1. Open an issue describing the proposed change.  
2. Fork the repository and create a feature branch.  
3. For mapping updates, include sources and a short justification explaining why a control maps to a specific SAFe phase.  
4. **Do not include proprietary text** from ISO/IEC, ITIL, or COBIT. Use identifiers and titles only.  
5. Add or adjust tests as applicable.  
6. Code of Conduct: see `CODE_OF_CONDUCT.md` (placeholder).

## Cite this work

If you use this repository, please cite the thesis and the software:

**Thesis (placeholders):**  
NAME, “Agile Control Map: Mapping Relevant IT Frameworks to Phases of Agile Solution Development (SAFe),” UNIVERSITY, CITY, YEAR, MONTH. Advisor: Edgar Weippl. Assistance: Alexander Schatten, Philipp Reisinger. URL: THESIS_URL_OR_REPO_URL.

**Software (placeholders):**  
Agile Control Map, version **VERSION**, released **RELEASE_DATE**, repository **REPO_URL**, DOI **DOI**.

## Acknowledgments

Developed as part of the master’s thesis by **Gerhard Schreihans**. Advisor: **Edgar Weippl**. Assistance: **Alexander Schatten** and **Philipp Reisinger**. Methodological underpinnings: **Kitchenham SLR** and **Hevner Design Science**.

## License

The Agile Control Map diagram (.drawio source, exported SVG/PNG) is licensed under the **Creative Commons Attribution–ShareAlike 4.0 International License (CC BY-SA 4.0)**.

You are free to:
- **Share** — copy and redistribute the material in any medium or format
- **Adapt** — remix, transform, and build upon the material for any purpose, even commercially

Under the following terms:
- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made.
- **ShareAlike** — If you remix, transform, or build upon the material, you must distribute your contributions under the **same license** as the original.
- **No additional restrictions** — You may not apply legal terms or technological measures that legally restrict others from doing anything the license permits.

Full legal text: [https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)

**Attribution example**:  
> Agile Control Map diagram by Gerhard Schreihans, licensed under CC BY-SA 4.0. Changes were made.

### Trademarks & proprietary standards
SAFe®, ITIL®, and COBIT® are trademarks of their respective owners.  
ISO/IEC standards text is proprietary. This repository references **identifiers and public metadata only** and does **not** redistribute standard contents or imply endorsement.

## Contact

- **Author:** NAME  
- **Email:** EMAIL  
- **LinkedIn:** LINKEDIN_URL  
- **Organization:** ORGANIZATION  
- **Repository:** REPO_URL  
- **Issues:** REPO_URL/issues

## Disclaimer

This artifact supports planning and governance in agile environments. It does not replace legal, regulatory, or auditor advice. Use at your own risk and validate mappings with your organization’s policies and standard licenses.
