<!-- omit in toc -->
# Quick Start Guide

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](README_FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](README.md)

---
<!-- omit in toc -->
## Table of Contents

- [About](#about)
- [Getting started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Become a member](#become-a-member)
  - [Create a new GitHub repository](#create-a-new-github-repository)
  - [Migrate an existing repository](#migrate-an-existing-repository)
  - [Develop the project](#develop-the-project)
  - [Publish a project](#publish-a-project)
    - [Before requesting publication](#before-requesting-publication)
      - [Form Completion Instructions](#form-completion-instructions)
    - [Requesting Publication](#requesting-publication)
    - [After Publication](#after-publication)
- [Learning resources](#learning-resources)
- [Acknowledgements](#acknowledgements)
- [Contribution](#contribution)
- [Security](#security)
- [License](#license)
- [Need Help?](#need-help)

---

## About

This repository serves as an onboarding reference for new and existing members of the *AAFC-Bioinfo-AAC* GitHub organization.

Membership and access to services are limited to AAFC employees and approved external collaborators via the AAFC partner.

Service requests and related notifications are managed through AAFC’s internal IT ticketing system, accessible via [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Guidance on the information required for each type of service request can be found in the [AAFC-Bioinfo-AAC GitHub Services Guide](./docs/aafc-bioinfo-aac-github-services-EN.md).

---

## Getting started

### Prerequisites

- Git installation: request via [My IT Centre TI → Other Software Requests](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHUZDIMJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=)
- GitHub account: If you don’t already have one, [create an account](https://github.com/signup).
- GitHub authentication: Interacting with Github through any method other than the web interface (e.g., using Git from the command line, GitHub CLI, IDE integrations, or GitHub Desktop) requires [account authentication](https://docs.github.com/en/authentication).

> [!TIP]
> If your existing GitHub account is primarily used for personal projects, consider creating a separate professional one for official work (e.g., `firstname-lastname-aafc`). According to the [Guide for Publishing Open Source Code](https://www.canada.ca/en/government/system/digital-government/digital-government-innovations/open-source-software/guide-for-publishing-open-source-code.html#:~:text=Identify%20as%20an%20employee%20of%20the%20Government%20of%20Canada,-Employees%20should%20use) employees should use their full name and Government of Canada email address for all code contributions to public repositories while acting within the scope of their duties or employment.

---

### Become a member

To join the *AAFC-Bioinfo-AAC* GitHub organization, submit an IT ticket via [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue → Account Management → Add new user*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Include the [required information](./docs/aafc-bioinfo-aac-github-services-EN.md#add-new-user) such as your GitHub account username and names of any existing repositories in the organization you need access to. Once approved, you’ll receive an invitation to join.

---

### Create a new GitHub repository

To start a new project, submit an IT ticket via [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue → Repository Management → Create a new private repository*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Provide [required information](./docs/aafc-bioinfo-aac-github-services-EN.md#create-a-new-private-repository) such as a repository name ([see naming conventions](./docs/repo-naming-style-guide.md)) and the admin responsible for that repo. A new private repository will then be created and initialized using the standard [*AAFC-Bioinfo-AAC* template](https://github.com/AAFC-Bioinfo-AAC/template-repository). The template may be modified to suit your project's requirements while keeping required sections intact.

The repo admin may add new users to the repo directly. However, if those users are AAFC employees not already a member of `AAFC-Bioinfo-AAC`, it is best that they become a member before being added to the project. This will ensure that they do not appear as `external collaborators`.

---

### Migrate an existing repository

Follow the process above to create a new repository, and then migrate your existing repo there, either by yourself or via an IT ticket: [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue → Other*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

---

### Develop the project

- Clone (download) the remote GitHub repo to your local computer and follow standard Git development practices: *Pull → Branch → Change → Commit → Push → PR → Review → Merge → Update → Repeat*

- Follow [coding best practices](./docs/coding-best-practices.md) and [Learning Resources](#learning-resources) on Git.

- Ensure no sensitive, confidential, or proprietary data is ever committed or pushed to the remote repository. Properly configure the `.gitignore` file to exclude those files from being tracked.

> [!IMPORTANT]
> **Do not** clone or store your working copy inside a folder synchronized by any cloud-storage service (e.g., OneDrive, Dropbox, Google Drive, iCloud, etc.). To prevent file corruption and performance issues, always keep your repositories in a non-synced location — for example, a local folder under `C:\Users\<username>` or within WSL (`/home/\<username>`).

---

### Publish a project

#### Before requesting publication

- Review and update your `README.md` and project documentation to ensure they accurately reflect the current state and purpose of your project.
  
- Ensure the following files (from the standard [*AAFC-Bioinfo-AAC* template](https://github.com/AAFC-Bioinfo-AAC/template-repository)) are completed or adapted to your project, following instructions provided within those files or in the relevant README section of the template:
  - `LICENSE`: The default license is **MIT** — replace it if necessary. An R Shiny tool, [*OSSLicensR*](https://websphn001.agr.gc.ca/OSSLicensR/), is available (internal access only) to guide selection of an appropriate license.
  - `CITATION.cff`: Supplies citation metadata to encourage proper attribution of your software or workflow when reused by others.
  - `dockstore.yml`: Provides metadata for publishing analytical workflows to [Dockstore](https://dockstore.org/) — a platform for sharing tools and pipelines built with CWL, WDL, Nextflow, Snakemake, or Galaxy. ***Delete this file if Dockstore publication does not apply to your project.***
  
- Complete the *Open-Source Development or Publication Approval Form* (refer [Form Completion Instructions](#form-completion-instructions)).

##### Form Completion Instructions

The project/repository maintainer should complete sections A and B of the *Open-Source Development or Publication Approval Form* ([internal access link](https://001gc.sharepoint.com/:b:/r/sites/50055/pap1/Open%20Source%20Software/STB%20Open%20source%20code%20approval%20form%20-%20EN.pdf)) and get it signed by the Associate Director of their Centre.

#### Requesting Publication

When your project is ready to be made public, submit an IT ticket via [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue → Repository Management → Publish a repository*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Provide [required information](./docs/aafc-bioinfo-aac-github-services-EN.md#publish-a-repository-make-public) and attach the completed *Open-Source Development or Publication Approval Form* (refer [Form Completion Instructions](#form-completion-instructions)).

After a successful security review and ISB Director approval, the repository will be published.

#### After Publication

- The repository’s URL becomes publicly accessible, so verify again that no sensitive information or internal data is exposed before announcing or sharing the link.
- Add or update [GitHub topics and keywords](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics) to improve discoverability.
- If the project includes an application or distributable component, create a formal release.  
  - Tag each release following [semantic versioning](https://semver.org/) (e.g., v1.0.0) to clearly communicate changes and maintain a predictable versioning history.
  - Optionally provide release notes summarizing key changes, fixes, or new features to help users understand what’s included in each version.
- Keep metadata, documentation and dependencies up to date.
- Continue governance: manage issues and pull requests following `AAFC-Bioinfo-AAC` contribution standards.
- Monitor repository insights (traffic, forks, citations) to measure engagement and plan improvements.
- If the repository becomes inactive, follow the repository lifecycle guidance for [archiving or deprecation](./docs/aafc-bioinfo-aac-github-services-EN.md#archive-or-deprecate-a-repository).

---

## Learning resources

- [Git tutorial by W3Schools](https://www.w3schools.com/git/default.asp)
- [Learn Git](https://git-scm.com/learn)
- [Get started with GitHub documentation](https://docs.github.com/en/get-started)

---

## Acknowledgements

This guide was developed by the `AAFC Bioinformatics Code Catalogue (ABCC)` project team.

🤖 This project includes content generated with the assistance of AI models. All AI-generated material has been reviewed, verified, and, where necessary, refined by the project team to ensure accuracy.

---

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
