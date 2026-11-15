<div align="center">

# Awesome Craft Malaysia [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open-source tools useful to Malaysian SMEs, with verified MyInvois support called out separately.

![Tools](https://img.shields.io/badge/tools-21-6366f1?style=for-the-badge)
[![Categories](https://img.shields.io/badge/categories-5-0ea5e9?style=for-the-badge)](#contents)
[![Combined stars](https://img.shields.io/badge/combined_stars-97.1k-f59e0b?style=for-the-badge&logo=github)](#-leaderboard)
[![Stars](https://img.shields.io/github/stars/EdisonTKPcom/Awesome-Craft-Malaysia?style=for-the-badge&color=22c55e)](https://github.com/EdisonTKPcom/Awesome-Craft-Malaysia/stargazers)
[![Last commit](https://img.shields.io/github/last-commit/EdisonTKPcom/Awesome-Craft-Malaysia?style=for-the-badge&color=ec4899)](https://github.com/EdisonTKPcom/Awesome-Craft-Malaysia/commits/main)

</div>

Official LHDN and IRBM documentation is a reference, not an open-source tool. Do not assume a generic ERP, POS or CRM is MyInvois-compliant or SST or EPF localized just because it is open source. For ERPNext, MyInvois support documented here is a separate Frappe app, not ERPNext core. For Odoo, official docs describe submission through Odoo registered as an intermediary on the taxpayer MyTax profile. This research did not find a clearly licensed, clearly maintained complete Malaysian statutory payroll package to list as verified.

Related lists: [Awesome Craft](https://github.com/EdisonTKPcom/Awesome-Craft).

## Contents

- [Dashboard](#dashboard)
- [Official references](#official-references)
- [Verified MyInvois integrations and SDKs](#verified-myinvois-integrations-and-sdks)
- [Verified Malaysia localization in Odoo](#verified-malaysia-localization-in-odoo)
- [Community documentation](#community-documentation)
- [Generic tools that need integration](#generic-tools-that-need-integration)

## Dashboard

<table>
<tr>
<td align="center"><h2>21</h2>listed projects</td>
<td align="center"><h2>5</h2>categories</td>
<td align="center"><h2>97.1k</h2>combined GitHub stars</td>
<td align="center"><h2>47.8k</h2>combined forks</td>
<td align="center"><h2>2/2</h2>pushed in the last 30 days</td>
<td align="center"><h2>1</h2>languages</td>
</tr>
</table>

Stats snapshot taken on 2026-11-15 from the GitHub API, for GitHub-hosted repositories only. Official documentation and other non-GitHub entries are listed but have no stars, forks or push dates. Star badges next to GitHub entries update live.

### 🏆 Leaderboard

<table>
<tr><th>Rank</th><th>Project</th><th>Kind</th><th align="right">Stars</th><th></th></tr>
<tr><td align="center">🥇</td><td><b>Odoo Community</b></td><td>ERP</td><td align="right">55.8k</td><td><code>████████████████████</code></td></tr>
<tr><td align="center">🥈</td><td><b>ERPNext</b></td><td>ERP</td><td align="right">41.3k</td><td><code>███████████████</code></td></tr>
</table>


### Stars by category

```mermaid
pie showData
    title Combined GitHub stars by category
    "Official references" : 0
    "Verified MyInvois integrations and SDKs" : 0
    "Verified Malaysia localization in Odoo" : 0
    "Community documentation" : 0
    "Generic tools that need integration" : 97108
```

### Licences

![GPL-3.0](https://img.shields.io/badge/GPL--3.0-1-64748b?style=flat-square) ![Custom](https://img.shields.io/badge/Custom-1-64748b?style=flat-square)

"Custom" or "None" means GitHub could not match a standard SPDX licence, often because of extra terms or an undeclared licence. Read the project licence before you use it commercially.

## Official references

- [LHDN](https://www.hasil.gov.my/) - The Malaysian tax authority site, including e-invoice guidelines and notices. Prefer current official guideline PDFs over third-party summaries.
- [MyInvois e-Invoice APIs](https://sdk.myinvois.hasil.gov.my/einvoicingapi/) - The official API reference for TIN validation, document submission, cancellation, rejection, retrieval, search and related operations.
- [MyInvois portal](https://myinvois.hasil.gov.my/) - The official taxpayer portal for the MyInvois system. Use the pre-production and production URLs published by LHDN for the environment you intend.
- [MyInvois SDK](https://sdk.myinvois.hasil.gov.my/) - Official LHDN documentation of the APIs taxpayer systems use to integrate with MyInvois.

## Verified MyInvois integrations and SDKs

- [danieyal/myinvois-python](https://github.com/danieyal/myinvois-python) - An unofficial Python SDK for MyInvois, including OAuth2, UBL 2.1 models, signing and submission. The README describes it as beta and not yet verified end-to-end against a live LHDN environment. ![Stars](https://img.shields.io/github/stars/danieyal/myinvois-python?style=flat-square&label=%E2%AD%90)
- [ERPGulf MyInvois](https://github.com/ERPGulf/myinvois) - A Frappe and ERPNext app that submits invoices and related document types to the MyInvois APIs. This is a separate app, not the ERPNext core repository. Test in LHDN pre-production before production use. ![Stars](https://img.shields.io/github/stars/ERPGulf/myinvois?style=flat-square&label=%E2%AD%90)
- [klsheng/myinvois-php-sdk](https://github.com/klsheng/myinvois-php-sdk) - A PHP client library for the MyInvois APIs. This is an SDK, not an accounting system; you still have to implement document mapping, signing and error handling. ![Stars](https://img.shields.io/github/stars/klsheng/myinvois-php-sdk?style=flat-square&label=%E2%AD%90)
- [Odoo Malaysia e-invoicing](https://github.com/odoo/odoo/tree/20.0/addons/l10n_my_edi) - The official Odoo l10n_my_edi module for submitting invoices to MyInvois. Official Odoo 20 docs say the taxpayer must add ODOO S.A. as a MyTax intermediary. The module is LGPL-3 in the Community tree.
- [Odoo Malaysia e-invoicing for POS](https://github.com/odoo/odoo/tree/20.0/addons/l10n_my_edi_pos) - The official Odoo l10n_my_edi_pos module for sending POS and consolidated POS invoices to MyInvois, using the same intermediary architecture. Confirm availability in your edition.
- [syukranDev/e-invoice-sdk-nodejs](https://github.com/syukranDev/e-invoice-sdk-nodejs) - A Node.js SDK aimed at LHDN e-invoicing and MyInvois. Verify against the current official API and pre-production before production use. ![Stars](https://img.shields.io/github/stars/syukranDev/e-invoice-sdk-nodejs?style=flat-square&label=%E2%AD%90)

## Verified Malaysia localization in Odoo

- [Odoo Malaysia Accounting](https://github.com/odoo/odoo/tree/20.0/addons/l10n_my) - The official l10n_my fiscal localization package. Odoo 20 docs describe default SST taxes and Malaysian company and product fields. This is fiscal localization, not by itself a complete MyInvois integration.
- [Odoo Malaysia Accounting Reports](https://github.com/odoo/odoo/tree/20.0/addons/l10n_my_reports) - Official Odoo 20 docs list SST-02 tax reports under l10n_my_reports. Many Odoo *_reports modules have historically shipped with Enterprise; confirm the edition you are licensed to run.
- [Odoo Malaysia UBL PINT](https://github.com/odoo/odoo/tree/20.0/addons/l10n_my_ubl_pint) - The official l10n_my_ubl_pint module, documented as providing features required to export invoices in PINT format.

## Community documentation

- [myinvois-docs](https://github.com/deadboy18/myinvois-docs) - Community-maintained developer documentation for MyInvois. It is not an official LHDN publication; re-verify operational details against official sources. ![Stars](https://img.shields.io/github/stars/deadboy18/myinvois-docs?style=flat-square&label=%E2%AD%90)

## Generic tools that need integration

- [Akaunting](https://github.com/akaunting/akaunting) - Self-hosted accounting. No MyInvois support is claimed here. ![Stars](https://img.shields.io/github/stars/akaunting/akaunting?style=flat-square&label=%E2%AD%90)
- [Chatwoot](https://github.com/chatwoot/chatwoot) - A self-hosted customer support inbox. WhatsApp access, when used, should go through Meta official Cloud or Business APIs and is subject to Meta terms. This is not a Malaysia-specific product. ![Stars](https://img.shields.io/github/stars/chatwoot/chatwoot?style=flat-square&label=%E2%AD%90)
- [Dolibarr](https://github.com/Dolibarr/dolibarr) - A modular open-source ERP and CRM. No verified MyInvois or Malaysian statutory module is claimed here. ![Stars](https://img.shields.io/github/stars/Dolibarr/dolibarr?style=flat-square&label=%E2%AD%90)
- [ERPNext](https://github.com/frappe/erpnext) - An open-source ERP with accounting, inventory, CRM and POS. Malaysia MyInvois support documented above is the ERPGulf app, not a feature verified here in ERPNext core. ![Stars](https://img.shields.io/github/stars/frappe/erpnext?style=flat-square&label=%E2%AD%90)
- [Frappe HR](https://github.com/frappe/hrms) - Open-source HR and payroll on the Frappe framework. No verified EPF, SOCSO, EIS or PCB implementation is claimed here. ![Stars](https://img.shields.io/github/stars/frappe/hrms?style=flat-square&label=%E2%AD%90)
- [Invoice Ninja](https://github.com/invoiceninja/invoiceninja) - Self-hosted invoicing and client billing. No MyInvois support is claimed here. ![Stars](https://img.shields.io/github/stars/invoiceninja/invoiceninja?style=flat-square&label=%E2%AD%90)
- [Odoo Community](https://github.com/odoo/odoo) - Open-source ERP, CRM, POS and accounting. Malaysia-specific behaviour should be taken from the verified modules above, not assumed for every official app. ![Stars](https://img.shields.io/github/stars/odoo/odoo?style=flat-square&label=%E2%AD%90)

## Contributing

Contributions welcome! Read the [contribution guidelines](contributing.md) first.

<div align="center">

If this list is useful, give it a ⭐ so others can find it.

</div>
