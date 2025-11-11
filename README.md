<!-- omit in toc -->
# Quick Start Guide

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](README_FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](README.md)

---
<!-- omit in toc -->
## Table of Contents

- [About](#about)
- [Getting started](#getting-started)
  - [Set up Git and GitHub](#set-up-git-and-github)
  - [Become a member](#become-a-member)
  - [Create or migrate a project](#create-or-migrate-a-project)
- [Develop the project](#develop-the-project)
  - [Publish a repository](#publish-a-repository)
- [Acknowledgements](#acknowledgements)
- [Contribution](#contribution)
- [Security](#security)
- [License](#license)
- [Need Help?](#need-help)

---

## About

This repository serves as an onboarding reference for new and existing members of the **AAFC-Bioinfo-AAC** GitHub organization.

Membership and access to services on **AAFC-Bioinfo-AAC** is limited to AAFC employees (and approved external collaborators via the AAFC partner).

Service requests and updates are handled through AAFC’s internal IT ticketing system: [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=)

See [AAFC-Bioinfo-AAC GitHub Services Guide](./docs/aafc-bioinfo-aac-github-services-EN.md) for a full list of service requests and details on information to include with each request.

## Getting started

### Set up Git and GitHub

A local Git installation (request via [My IT Centre TI → Other Software Requests](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHUZDIMJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=)) and proper [GitHub authentication](https://docs.github.com/en/authentication) setup will be required to interact with Github through any method (e.g., using Git from the command line, GitHub CLI, IDE integrations, or GitHub Desktop) other than the web interface.

If you also use GitHub for personal projects, consider creating a separate account for official work. According to the [Guide for Publishing Open Source Code](https://www.canada.ca/en/government/system/digital-government/digital-government-innovations/open-source-software/guide-for-publishing-open-source-code.html#:~:text=of%20your%20code.-,Identify%20as%20an%20employee%20of%20the%20Government%20of%20Canada,-Employees%20should%20use) employees should use their full name and Government of Canada email address for all code contributions to public repositories while acting within the scope of their duties or employment.

### Become a member

To join as a member of **AAFC-Bioinfo-AAC**, submit an IT ticket under **Account Management → Add new user**, providing [details](./docs/aafc-bioinfo-aac-github-services-EN.md#add-new-user) such as your GitHub username and names of any existing repos you wish to be added to.

### Create or migrate a project

To start a project afresh on **AAFC-Bioinfo-AAC** or to migrate an existing project from elsewhere, submit an IT ticket under **Repository Management → Create a new private repository**, providing [details](./docs/aafc-bioinfo-aac-github-services-EN.md#create-a-new-private-repository) such as a project name ([see naming conventions](./docs/repo-naming-style-guide.md)) and project admin. A new private repo will be created and initialised with a [template](https://github.com/AAFC-Bioinfo-AAC/template-repository). The template may be modified to suit your requirements for the new or migrated project while keeping the content in the required sections.

New users may be added to the project directly by the project admin. However, if that user is an AAFC employee and not already a member of the org, it is best that the user submit an IT ticket to be added to the project. This will ensure that the user does not appear as an external collaborator.

---

## Develop the project

Follow [coding best practices](./docs/coding-best-practices.md) and ensure no sensitive, confidential, or proprietary data should are uploaded. Some learning resources:

- [Learn Git](https://git-scm.com/learn)
- [Get started with GitHub](https://docs.github.com/en/get-started)
- [Git tutorial by w3schools](https://www.w3schools.com/git/default.asp)

### Publish a repository

When ready to publish a repo, submit an IT ticket under **Repository Management → Publish a repository**, providing [details](./docs/aafc-bioinfo-aac-github-services-EN.md#publish-a-repository-make-public) requested and including a completed [Open-Source Development or Publication Approval Form](https://001gc.sharepoint.com/:w:/r/sites/50055/pap1/Open%20Source%20Software/STB%20Open%20source%20code%20approval%20form%20-%20EN.docx) (internal access only). The repo will be published following an internal security review process.

For best practices, ensure the following files included in the template repo (with instructions on how to fill) are completed/adapted prior to requesting publication:

- LICENSE: default MIT is included in the template. An interactive R Shiny application [OSSLicensR](https://websphn001.agr.gc.ca/OSSLicensR/) (internal access only) is available to help select an appropriate open-source or source-available license for their software project.
- dockstore.yml: Applies only for workflows in CWL, WDL, Nextflow, Snakemake or Galaxy. Delete if not.
- CITATION.cff

---

## Acknowledgements

This guide was developed by the **ABCC project team**.

🤖 This project includes content generated with the assistance of AI models. All AI-generated material has been reviewed, verified, and, where necessary, refined by the project team to ensure accuracy.

## Contribution

Contributions are welcome! Please review the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md) and ensure you adhere to our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) to foster a respectful and inclusive environment.

---

## Security  

⚠️ Do not post any security issues on the public repository! Please report them as described in [SECURITY.md](SECURITY.md)

---

## License

See the [LICENSE](LICENSE) file for details. Visit [LicenseHub](https://licensehub.org) or [tl;drLegal](https://www.tldrlegal.com/) to view a plain-language summary of this license.

**Copyright ©** His Majesty the King in Right of Canada, as represented by the Minister of Agriculture and Agri-Food, 2025.

---

## Need Help?

Email [BRSN](mailto:aafc.bioinfosupport.aac@agr.gc.ca) with subject: `AAFC-Bioinfo-AAC: <summary>`
