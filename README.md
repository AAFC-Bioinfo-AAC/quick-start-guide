<!-- omit in toc -->
# Quick Start Guide

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](README_FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](README.md)

---
<!-- omit in toc -->
## Table of Contents

- [About](#about)
- [Getting started](#getting-started)
  - [Become a member](#become-a-member)
  - [Create a new project](#create-a-new-project)
  - [Migrate an existing project](#migrate-an-existing-project)
  - [Develop the project locally](#develop-the-project-locally)
  - [Publish a project](#publish-a-project)
    - [Before requesting publication](#before-requesting-publication)
    - [After Publication](#after-publication)
- [Acknowledgements](#acknowledgements)
- [Contribution](#contribution)
- [Security](#security)
- [License](#license)
- [Need Help?](#need-help)

---

## About

This repository serves as an onboarding reference for new and existing members of the *AAFC-Bioinfo-AAC* GitHub organization.

Membership and access to services on *AAFC-Bioinfo-AAC* is limited to AAFC employees and approved external collaborators via the AAFC partner.

Service requests and related notifications are managed through AAFC’s internal IT ticketing system, accessible via [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Guidance on the information required for each type of service request can be found in the [AAFC-Bioinfo-AAC GitHub Services Guide](./docs/aafc-bioinfo-aac-github-services-EN.md).

---

## Getting started

### Become a member

To join the *AAFC-Bioinfo-AAC* GitHub organization, submit an IT ticket through [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue → Account Management → Add new user*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Include the [required information](./docs/aafc-bioinfo-aac-github-services-EN.md#add-new-user) such as your GitHub account username ([create one here](https://github.com/signup) if you don’t already have) and names of any existing repositories in the organization you need access to. Once approved, you’ll receive an invitation the organization.

> [!TIP]
> If your existing GitHub account is primarily used for personal projects, consider creating a separate one for official work, choosing a clear, professional GitHub username, such as `firstname-lastname-aafc`. According to the [Guide for Publishing Open Source Code](https://www.canada.ca/en/government/system/digital-government/digital-government-innovations/open-source-software/guide-for-publishing-open-source-code.html#:~:text=of%20your%20code.-,Identify%20as%20an%20employee%20of%20the%20Government%20of%20Canada,-Employees%20should%20use) employees should use their full name and Government of Canada email address for all code contributions to public repositories while acting within the scope of their duties or employment.

---

### Create a new project

To start a new project, submit an IT ticket through [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue → Repository Management → Create a new private repository*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=), providing [required information](./docs/aafc-bioinfo-aac-github-services-EN.md#create-a-new-private-repository) such as a project name ([see naming conventions](./docs/repo-naming-style-guide.md)) and project admin. A new private repository will then be created and initialized using the standard [*AAFC-Bioinfo-AAC* template](https://github.com/AAFC-Bioinfo-AAC/template-repository).

New users may be added to the project directly by the project admin. However, if that user is an AAFC employee and not already a member of the org, it is best that the user submit an IT ticket to be added to the project. This will ensure that the user does not appear as an external collaborator.

---

### Migrate an existing project

Follow the process above to create a new project and the migrate your existing project there, either by yourself, or via an IT ticket through [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue → Other*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

---

### Develop the project locally

Follow the steps described in this [document](./docs/developing-locally.md) to clone the project to your local machine, make changes safely, and contribute via pull requests. The template may be modified to suit your requirements for the new or migrated project while keeping the content in the required sections. Ensure no sensitive, confidential, or proprietary data are uploaded and follow [coding best practices](./docs/coding-best-practices.md).

Some learning resources:

- [Learn Git](https://git-scm.com/learn)
- [Get started with GitHub](https://docs.github.com/en/get-started)
- [Git tutorial by w3schools](https://www.w3schools.com/git/default.asp)

Prerequisites:

- **Git** installation (request via [My IT Centre TI → Other Software Requests](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHUZDIMJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=))
- **GitHub account** with access to the repository.
- **Authentication** set up (HTTPS with Personal Access Token, or SSH keys). [GitHub authentication](https://docs.github.com/en/authentication) will be required to interact with Github through any method (e.g., using Git from the command line, GitHub CLI, IDE integrations, or GitHub Desktop) other than the web interface.
- **Language runtime/tools** for this project (e.g., Python/Node/Java) and any package manager (pip/npm/maven/etc.).

> [!IMPORTANT]
> Do **not** clone/place your working copy inside OneDrive sync folders. Keep repos in a sync excluded folder within OneDrive or a folder outside of OneDrive like `C:\Users\<username>` (or your WSL home) to avoid corruption and performance issues.

---

### Publish a project

When your project is ready to be made public, submit an IT ticket through [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue → Repository Management → Publish a repository*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=), providing [required information](./docs/aafc-bioinfo-aac-github-services-EN.md#publish-a-repository-make-public) and attaching a completed [*Open-Source Development or Publication Approval Form*](https://001gc.sharepoint.com/:w:/r/sites/50055/pap1/Open%20Source%20Software/STB%20Open%20source%20code%20approval%20form%20-%20EN.docx) (internal access only). The repository will undergo an internal security review process clearing which it will be made public.

#### Before requesting publication

Review and update your `README.md` and project documentation before publication to ensure it accurately reflects the current state and purpose of your project.

Also ensure the following files included in the the standard [*AAFC-Bioinfo-AAC* template](https://github.com/AAFC-Bioinfo-AAC/template-repository) are completed or adapted for your project, following instructions provided within those files or in the relevant README section:

| File | Purpose / Notes |
| ----- | --------------- |
| dockstore.yml | Provides metadata for publishing analytical workflows to [Dockstore](https://dockstore.org/) — a platform for sharing tools and pipelines built with CWL, WDL, Nextflow, Snakemake, or Galaxy. <br>*\*Delete this file if Dockstore publication does not apply to your project.*|
| CITATION.cff| Supplies citation metadata to encourage proper attribution of your software or workflow when reused by others.|
| `LICENSE` | The default license is **MIT** — replace it if necessary. <br> *\*An internal R Shiny tool, *OSSLicensR* (internal access only), is available to help you select an appropriate license.* |

#### After Publication

Once your repository has passed the internal review and been published:

1. **Repository visibility**  
   - The repository will be switched from **private** to **public** within the **AAFC-Bioinfo-AAC** GitHub organization.  
   - The repository’s URL will become accessible to external users.  
   - Contributors should confirm that no sensitive information (e.g., credentials, API keys, internal endpoints) remains in the commit history or files.

2. **Repository metadata and documentation**  
   - Verify that your `README.md` clearly describes the project’s purpose, installation steps, and usage examples.  
   - Ensure `LICENSE`, `CITATION.cff`, and `dockstore.yml` (if applicable) are complete and accurate.  
   - Add or update your project’s **keywords** and **topics** on GitHub to improve discoverability.

3. **Acknowledgment and attribution**  
   - Encourage users to cite your project using the information in `CITATION.cff`.  
   - If your project will be shared on other platforms (e.g., Dockstore, Zenodo, or AAFC websites), include the GitHub link in those metadata records.

4. **Maintenance and governance**  
   - Continue to manage issues and pull requests following AAFC-Bioinfo-AAC contribution standards.  
   - Tag releases using [semantic versioning](https://semver.org/) (e.g., `v1.0.0`) to track changes and enable reproducibility.  
   - Keep documentation and dependencies up to date.  
   - Archive or deprecate the repository if it becomes inactive, following the [repository lifecycle guidance](./docs/aafc-bioinfo-aac-github-services-EN.md#archive-or-deprecate-a-repository).

> [!TIP]  
> After publication, monitor repository insights such as **traffic**, **forks**, and **citations** to measure engagement and plan future improvements.  
> Consider adding a **CHANGELOG.md** to document major updates over time.

---

## Acknowledgements

This guide was developed by the **ABCC project team**.

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
