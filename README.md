# Agile Control Map (ACM)

> Map relevant IT frameworks (ITIL, COBIT, CIS Controls, ISO/IEC 27001/27002) to phases of agile solution development (SAFe) so teams can move fast and not break things.

![Status](https://img.shields.io/badge/status-research%20artifact-informational)
[![License: CC BY-SA 4.0](https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-sa/4.0/)
![SAFe](https://img.shields.io/badge/framework-SAFe%206.0-2ea44f)
![Standards](https://img.shields.io/badge/refs-ITIL%204%20%7C%20COBIT%202019%20%7C%20ISO%2FIEC%2027001:2022%2F27002:2022%20%7C%20CIS%20Controls%20v8.1-8a2be2)

<details>
<summary><strong>Table of contents</strong></summary>

- [Overview](#overview)
- [Why this exists](#why-this-exists)
- [What the artifact does](#what-the-artifact-does)
- [Background &amp; scope](#background--scope)
- [Methodology](#methodology)
- [Usage](#usage)
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

**Project context:** Master’s thesis “Move Fast and Don’t Break Things — Mapping Relevant IT Frameworks (ITIL, COBIT, CIS Controls, ISO/IEC 27001/27002) to Phases of Agile Solution Development (SAFe)” by **Gerhard Schreihans**. 
Advisor: **Edgar Weippl**. 
Assistance: **Alexander Schatten**, **Philipp Reisinger**.

## Why this exists

Teams often overlook framework-driven requirements such as backups or segregation of duties because they do not add immediate user-facing functionality and therefore rarely become stories. The result can be security and quality gaps, especially across non-functional requirements. ACM surfaces these requirements at the right time in SAFe, so they can be sized and scheduled like any other work.

## What the artifact does

- Maps SAFe phases and activities to relevant practices and controls from **ITIL 4**, **COBIT 2019**, **ISO/IEC 27001:2022 & 27002:2022**, and **CIS Controls v8.1**.
- Highlights candidate inputs for **enabler** and **user stories** derived from those controls.

## Background & scope

**Problem space:** Larger, regulated organizations want the speed of agile-organized organizations while maintaining robust Internal Control Systems; regulators require resilient governance and controls. ACM addresses the friction between value creation (agile) and risk reduction (governance).

**In-scope frameworks:** SAFe 6.0 as process backbone with mappings to ITIL 4, COBIT 2019, ISO/IEC 27001:2022/27002:2022, and CIS Controls v8.1.

**Scope statement:** ACM does not invent a new framework; it uses existing ones to guide when specific controls and process steps should be considered.

## Methodology

- **Systematic Literature Review** based on Kitchenham guidelines to collect and assess evidence on combining agile methods with IT frameworks.
- **Design Science approach (Hevner):** artifact design, ex-ante validation via expert interviews, and ex-post naturalistic evaluation via a broader expert survey. The artifact is considered acceptable if a majority evaluates it positively.

## Usage

- Explore which controls are relevant for a given SAFe phase or activity.  
- Derive enabler and user stories from mapped controls and include them in planning and refinement.  
- Share exports with teams for PI planning, governance reviews, or audits.  
- Capture organizational adaptations and rationales alongside the mapping.

## Contributing

Contributions are welcome.

1. Open an issue describing the proposed change.  
2. Fork the repository and create a feature branch.  
3. For mapping updates, include sources and a short justification explaining why a control maps to a specific SAFe phase.  
4. **Do not include proprietary text** from ISO/IEC, ITIL, or COBIT. Use identifiers, titles or very selective parts of the documents only.  
5. Add or adjust tests as applicable. 

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

- **Author:** Gerhard Schreihans  
- **Email:** ![gerhard.schreihans@aubotics.com](mailto:gerhard.schreihans@aubotics.com)
- **LinkedIn:** [https://www.linkedin.com/in/gerhard-schreihans-7599b693/](https://www.linkedin.com/in/gerhard-schreihans-7599b693/)

## Disclaimer

This artifact supports planning and governance in agile environments. It does not replace legal, regulatory, or auditor advice. Use at your own risk and validate mappings with your organization’s policies and standard licenses.
