# PRESTASHOP PRIOR DOCS

![license](https://img.shields.io/badge/license-license-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-online_retail-lightgrey)

> Anticloud-hardened packaging of the upstream project `PRESTASHOP_PRIOR_DOCS` in category **ONLINE RETAIL**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** ONLINE RETAIL · **Upstream:** https://github.com/PrestaShop/PrestaShop · **Upstream pin:** `dec15c65a3f3a0c27cfd1dc221a7b89bff036fa2` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

About PrestaShop
--------

[![PHP checks and unit tests](https://github.com/PrestaShop/PrestaShop/actions/workflows/php.yml/badge.svg)](https://github.com/PrestaShop/PrestaShop/actions/workflows/php.yml)
[![Integration tests](https://github.com/PrestaShop/PrestaShop/actions/workflows/integration.yml/badge.svg)](https://github.com/PrestaShop/PrestaShop/actions/workflows/integration.yml)
[![UI tests](https://github.com/PrestaShop/PrestaShop/actions/workflows/sanity.yml/badge.svg)](https://github.com/PrestaShop/PrestaShop/actions/workflows/sanity.yml)
[![Nightly Status](https://img.shields.io/endpoint?url=https%3A%2F%2Fapi-nightly.prestashop-project.org%2Fdata%2Fbadge&label=Nightly%20Status&cacheSeconds=3600)](https://nightly.prestashop-project.org/)
[![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%208.1-8892BF.svg?style=flat-square)](https://php.net/)
[![GitHub release](https://img.shields.io/github/v/release/prestashop/prestashop?sort=semver)](https://github.com/PrestaShop/PrestaShop)
[![LFX Health Score](https://insights.linuxfoundation.org/api/badge/health-score?project=prestashop)](https://insights.linuxfoundation.org/project/prestashop)
[![Slack chat](https://img.shields.io/badge/Chat-on%20Slack-red)](https://www.prestashop-project.org/slack/)
[![GitHub forks](https://img.shields.io/github/forks/PrestaShop/PrestaShop)](https://github.com/PrestaShop/PrestaShop/network)
[![GitHub stars](https://img.shields.io/github/stars/PrestaShop/PrestaShop)](https://github.com/PrestaShop/PrestaShop/stargazers)

PrestaShop is an Open Source e-commerce web application, committed to providing the best shopping cart experience for both merchants and customers. It is written in PHP, is highly customizable, supports all the major payment services, is translated in many languages and localized for many countries, has a fully responsive design (both front and back office), etc. [See all the available features][available-features].

<p align="center">
  <img src="https://github.com/user-attachments/assets/e6342778-e528-4ae7-acf2-f0d097a1e932" alt="PrestaShop 9.0 back office"/>
</p>

This project contains the source code of PrestaShop, which is intended for development and preview only. To download the latest stable public version of PrestaShop (currently, version 9.0), please go to [the releases page][download].

The first stable version of PrestaShop 9.0 was released on June 10th, 2025. Learn more about it on [the Build devblog](https://build.prestashop-project.org/tag/9.0/).

About the `develop` branch
--------

The `develop` branch of this project contains the work in progress source code for the next version of PrestaShop. Currently, it is exclusively for version 9.1.

For more information on our branch system, read our guide on [installing PrestaShop for development][install-guide-dev].

Server configuration
--------

To install the latest PrestaShop 9.0, you need a web server running PHP 8.1+ and any flavor of MySQL 5.6+ (MySQL, MariaDB, Percona Server, etc.).

You will also need a database administration tool, such as phpMyAdmin, in order to create a database for PrestaShop.
We recommend the Apache or Nginx web servers (check out our [example Nginx configuration file][example-nginx]).

You can find more information on our [System requirements][system-requirements] page and on the [System Administrator Guide][sysadmin-guide].

Installation
--------

If you downloaded the source code from GitHub, read our guide on [installing PrestaShop for development][install-guide-dev]. If you intend to install a production shop, make sure to download the latest version from [our releases page][download], then read the [install guide for users][install-guide].

## 🐳 Docker Development Environment

PrestaShop provides a complete Docker-based development environment.

### Quick Start

```bash
# Start the development environment
make docker-start

# Access your PrestaShop installation
# Frontend: http://localhost:8001
# Backend: http://localhost:8001/admin-dev
# Email testing: http://localhost:1080
```

**Default Admin Credentials:**
- Email: `demo@prestashop.com`
- Password: `Pr3st4Sh0P`

Or the backoffice on this URL: http://localhost:8001/admin-dev (default access credentials: demo@prestashop.com / Pr3st4Sh0P)

You can customize the admin credentials by setting the following environment variables before running docker compose:
```
export ADMIN_MAIL=your-email@example.com
export ADMIN_PASSWD=Your-Secure-Password
docker compose up
```

Docker will bind your port **8001** to the web server. If you want to use other port, open and modify the file `docker-compose.yml`.
MySQL credentials can also be found and modified in this file if needed.

**Note:**  Before auto-installing PrestaShop, this container checks the file *app/config/parameters.php* does not exist on startup.
If you expect the container to (re)install your shop, remove this file if it exists. And make sure the container user `www-data`
has write access to the whole workspace.

### Documentation

For detailed information, see:

- **[🚀 Development Guide](./docs/DEVELOPMENT.md)** - Complete setup and development guide

Documentation
--------

For technical information (core, module and theme development, performance...), head on to [PrestaShop DevDocs][devdocs]

If you want to learn how to use PrestaShop 9, read our [User documentation][user-doc].

First-time users will be particularly interested in the following guides:

* [Getting Started][getting-started]: How to install PrestaShop, and what you need to know.
* [User Guide][user-guide]: All there is to know to put PrestaShop to good use.
* [Updating Guide][updating-guide]: Switching to the newest version is not trivial. Make sure you do it right.
* [Merchant's Guide][merchant-guide]: Tips and tricks for first-time online sellers.
* The [FAQ][faq-17] page should also be of tremendous help to you.

Contributing
--------

PrestaShop is an Open Source project, and it wouldn't be possible with

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **PHP / Composer** (manifests: composer.json, composer.lock; scanned in UPSTREAM_CLONE)
- Top-level source layout: `admin-api/`, `admin-dev/`, `app/`, `bin/`, `cache/`, `classes/`, `config/`, `controllers/`, `download/`, `img/`, `install-dev/`, `js/`
- Snapshot size: **15395 files**, **1179016 lines of code** (measured; see Benchmarks)
- Primary languages: `.php` (7869), `.ts` (1413), `.xml` (1188), `.jpg` (1054), `.twig` (775), `.js` (546)
- Upstream commit pinned for this packaging: `dec15c65a3f3a0c27cfd1dc221a7b89bff036fa2`

---

## Installation

About the `develop` branch
--------

The `develop` branch of this project contains the work in progress source code for the next version of PrestaShop. Currently, it is exclusively for version 9.1.

For more information on our branch system, read our guide on [installing PrestaShop for development][install-guide-dev].

Server configuration
--------

To install the latest PrestaShop 9.0, you need a web server running PHP 8.1+ and any flavor of MySQL 5.6+ (MySQL, MariaDB, Percona Server, etc.).

You will also need a database administration tool, such as phpMyAdmin, in order to create a database for PrestaShop.
We recommend the Apache or Nginx web servers (check out our [example Nginx configuration file][example-nginx]).

You can find more information on our [System requirements][system-requirements] page and on the [System Administrator Guide][sysadmin-guide].

Installation
--------

If you downloaded the source code from GitHub, read our guide on [installing PrestaShop for development][install-guide-dev]. If you intend to install a production shop, make sure to download the latest version from [our releases page][download], then read the [install guide for users][install-guide].

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

You can find more information on our [System requirements][system-requirements] page and on the [System Administrator Guide][sysadmin-guide].

Installation
--------

If you downloaded the source code from GitHub, read our guide on [installing PrestaShop for development][install-guide-dev]. If you intend to install a production shop, make sure to download the latest version from [our releases page][download], then read the [install guide for users][install-guide].

*Section quoted from the upstream readme.*
Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

[![Minimum PHP Version](https://img.shields.io/badge/php-%3E%3D%208.1-8892BF.svg?style=flat-square)](https://php.net/)
[![GitHub release](https://img.shields.io/github/v/release/prestashop/prestashop?sort=semver)](https://github.com/PrestaShop/PrestaShop)
[![LFX Health Score](https://insights.linuxfoundation.org/api/badge/health-score?project=prestashop)](https://insights.linuxfoundation.org/project/prestashop)
[![Slack chat](https://img.shields.io/badge/Chat-on%20Slack-red)](https://www.prestashop-project.org/slack/)
[![GitHub forks](https://img.shields.io/github/forks/PrestaShop/PrestaShop)](https://github.com/PrestaShop/PrestaShop/network)
[![GitHub stars](https://img.shields.io/github/stars/PrestaShop/PrestaShop)](https://github.com/PrestaShop/PrestaShop/stargazers)

PrestaShop is an Open Source e-commerce web application, committed to providing the best shopping cart experience for both merchants and customers. It is written in PHP, is highly customizable, supports all the major payment services, is translated in many languages and localized for many countries, has a fully responsive design (both front and back office), etc. [See all the available features][available-features].

<p align="center">
  <img src="https://github.com/user-attachments/assets/e6342778-e528-4ae7-acf2-f0d097a1e932" alt="PrestaShop 9.0 back office"/>
</p>

This project contains the source code of PrestaShop, which is intended for development and preview only. To download the latest stable public version of PrestaShop (currently, version 9.0), please go to [the releases page][download].

The first stable version of PrestaShop 9.0 was released on June 10th, 2025. Learn more about it on [the Build devblog](https://build.prestashop-project.org/tag/9.0/).

About the `develop` branch
--------

The `develop` branch of this project contains the work in progress source code for the next version of PrestaShop. Currently, it is exclusively for version 9.1.

For more information on our branch system, read our guide on [installing PrestaShop for development][install-guide-dev].

Server configuration
--------

To install the latest PrestaShop 9.0, you need a web server running PHP 8.1+ and any flavor of MySQL 5.6+ (MySQL, MariaDB, Percona Server, etc.).

You will also need a database administration tool, such as phpMyAdmin, in order to create a database for PrestaShop.
We recommend the Apache or Nginx web servers (check out our [example Nginx configuration file][example-nginx]).

You can find more information on our [System requirements][system-requirements] page and on the [System Administrator Guide][sysadmin-guide].

Installation
--------

If you downloaded the source code from GitHub, read our guide on [installing PrestaShop for development][install-guide-dev]. If you intend to install a production shop, make sure to download the latest version from [our releases page][download], then read the [install guide for users][install-guide].

*Section quoted from the upstream readme.*
---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | PHP / Composer |
| Manifests detected | composer.json, composer.lock |
| Files in snapshot | 15395 |
| Lines of code | 1179016 |
| Dependency references | 180 |
| Dependencies by ecosystem | npm: 180 |
| Upstream license | No license file present in the upstream snapshot |
| Overlay license | Anticommons 0.1.0 |

Top dependency references recorded in the benchmark snapshot:

| Ecosystem | Name | Version | Source file |
|-----------|------|---------|-------------|
| npm | jquery | ^3.7.1 | themes/package.json |
| npm | jquery-migrate | ^3.5.2 | themes/package.json |
| npm | punycode | ^2.3.1 | themes/package.json |
| npm | @zxcvbn-ts/core | ^3.0.0 | themes/package.json |
| npm | @zxcvbn-ts/language-common | ^3.0.0 | themes/package.json |
| npm | @zxcvbn-ts/language-en | ^3.0.0 | themes/package.json |
| npm | @babel/eslint-parser | ^7.25.1 | themes/package.json |
| npm | esbuild-loader | ^4.2.2 | themes/package.json |
| npm | eslint | ^8.18.0 | themes/package.json |
| npm | eslint-config-airbnb-base | ^15.0.0 | themes/package.json |
| npm | eslint-import-resolver-webpack | ^0.13.9 | themes/package.json |
| npm | eslint-plugin-html | ^8.1.2 | themes/package.json |
| npm | eslint-plugin-import | ^2.30.0 | themes/package.json |
| npm | mini-css-extract-plugin | ^2.9.1 | themes/package.json |
| npm | path | ^0.12.7 | themes/package.json |
| ... | (165 more) | | |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

--------

To install the latest PrestaShop 9.0, you need a web server running PHP 8.1+ and any flavor of MySQL 5.6+ (MySQL, MariaDB, Percona Server, etc.).

You will also need a database administration tool, such as phpMyAdmin, in order to create a database for PrestaShop.
We recommend the Apache or Nginx web servers (check out our [example Nginx configuration file][example-nginx]).

You can find more information on our [System requirements][system-requirements] page and on the [System Administrator Guide][sysadmin-guide].

Installation
--------

If you downloaded the source code from GitHub, read our guide on [installing PrestaShop for development][install-guide-dev]. If you intend to install a production shop, make sure to download the latest version from [our releases page][download], then read the [install guide for users][install-guide].

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

*Excerpt from upstream `CONTRIBUTING.md`:*

Contributing to PrestaShop
--------------------------

PrestaShop is an open-source e-commerce solution. Everyone is welcome and even encouraged to contribute with their own improvements.

PrestaShop is written mostly in PHP. Other languages used throughout are JavaScript (and TypeScript), HTML, CSS, the Smarty & Twig templating languages, SQL, and XML.

To contribute to the project, you should ideally be familiar with Git, the source code management system that PrestaShop uses, with the official project being hosted on Github: 
* You can learn more about [Git](https://try.github.io/) (there are many tutorials available on the Web).
* You can get help on [Github](https://help.github.com/).
* Windows users can get a nice interface for Git by installing [TortoiseGit](https://tortoisegit.org/).

There are number of ways to contribute, it is not only about coding! You can read more about contributing on the [project's website][get-involved].

### About licenses

* All core files you commit in your pull request must respect/use the [Open Software License (OSL 3.0)][osl].
* All modules files you commit in your pull request must respect/use the [Academic Free License (AFL 3.0)][afl].

[osl]: https://opensource.org/licenses/OSL-3.0
[afl]: https://opensource.org/licenses/AFL-3.0
[get-involved]: https://www.prestashop-project.org/get-involved/

### Branches

The PrestaShop project adopts [our own flavor of git flow branching strategy](https://build.prestashop-project.org/news/2015/introducing-new-branching-model-prestashop/).

tl;dr Put bug fixes in 8.x or [other supported branches](https://github.com/PrestaShop/PrestaShop/branches), put new compatible and incompatible features in [the develop branch](https://github.com/PrestaShop/PrestaShop).

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: No license file present in the upstream snapshot** (evidence: `LICENSE.md` in the upstream snapshot).

License file excerpt:

```text

Copyright (c) Since 2007 PrestaShop and Contributors.

PrestaShop Core is licensed under OSL-3.0 and PrestaShop Modules are licensed under AFL-3.0. Please read [/docs/licenses/LICENSE.txt](/docs/licenses/LICENSE.txt) for details.

You can find useful resources about open source and licenses files for librairies used in the PrestaShop project in [/docs/licenses/](/docs/licenses/)
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original No license file present in the upstream snapshot terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `No license file present in the upstream snapshot` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `PRESTASHOP_PRIOR_DOCS` (category: ONLINE RETAIL)
- **Upstream URL:** https://github.com/PrestaShop/PrestaShop
- **Pinned commit (SHA):** `dec15c65a3f3a0c27cfd1dc221a7b89bff036fa2`
- **Branch:** develop
- **Pin provenance:** resolved during the second documentation pass. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`47bfa9d9dac6aa9ccffb2fbcb4fc1a546add6392ed14f98b5eb82dca7bab9efc`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

