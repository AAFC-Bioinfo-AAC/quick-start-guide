<!-- omit in toc -->
# Quick Start Guide

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](README_FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](https://github.com/AAFC-Bioinfo-AAC/quick-start-guide)

<!-- omit in toc -->
## About

This guide describes available services and recommended processes to manage and contribute to bioinformatics code repositories within the **AAFC-Bioinfo-AAC** GitHub organization, associated with the AAFC Bioinformatics Code Catalogue (ABCC) project.

<!-- omit in toc -->
## Table of Contents

- [*AAFC-Bioinfo-AAC* GitHub services](#aafc-bioinfo-aac-github-services)
  - [1. Repository Management](#1-repository-management)
    - [1.1. Create a new private repository](#11-create-a-new-private-repository)
    - [1.2. Publish a repository (make Public)](#12-publish-a-repository-make-public)
    - [1.3. Delete/Archive/Deprecate repository](#13-deletearchivedeprecate-repository)
  - [2. Account Management](#2-account-management)
    - [2.1. Add New User](#21-add-new-user)
    - [2.2. Remove User](#22-remove-user)
    - [2.3. Modify User Privileges](#23-modify-user-privileges)
  - [3. Training](#3-training)
  - [4. Other](#4-other)
- [Credits](#credits)
- [Citation](#citation)
- [Contribution](#contribution)
- [Security](#security)
- [License](#license)
- [Need Help?](#need-help)

---

## *AAFC-Bioinfo-AAC* GitHub services

The following services are available via `My IT Centre TI` under category: `Science IT Support > AAFC Bioinformatics Code Catalogue` ([internal access link](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=)).

### 1. Repository Management

#### 1.1. Create a new private repository

To initiate a new project or migrate an existing one to the `AAFC-Bioinfo-AAC` GitHub organization, click **Create a new private repository** and complete the form with:

- A repository name following [AAFC-Bioinfo-AAC repository naming conventions](./docs/repo-naming-style-guide.md).
- A brief bilingual description (English and French)
- Repository admin’s name, official email, GitHub username, and supervisor’s email
- If applicable, a list of team members with their names, email, GitHub username and assigned roles (admin, maintain, write, or read; refer [role permissions guide](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#permissions-for-each-role))

Important Notes:

- At least one user must be assigned the admin role.
- The admin is responsible for ongoing repository maintenance and user management.
- Contributors must follow [coding best practices](./docs/coding-best-practices.md).
- Additional users can be added later by the admin. If a user is not yet part of the organization, use the [Add new user](./README.md#21-add-new-user) form to ensure proper onboarding.

Once approved, the repository will be initialized from the standard template, including:

- Bilingual README templates with guidance and examples
- MIT License with Crown copyright
- Standard documents: `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, etc.

#### 1.2. Publish a repository (make Public)

To request that a repository be made public, click **Publish a repository** and provide:

- Repository name
- Repository admin's name, official email, GitHub username and supervisor's email
- A completed **Open-Source Development or Publication Approval Form** (link to form is provided in the ticket), signed by the Associate Director of your centre

After a successful security review and ISB Director approval, the repository will be published.

#### 1.3. Delete/Archive/Deprecate repository

To change the status of a repository, click **Delete/Archive/Deprecate repository** and submit the following:

- Desired action:
  - Delete: Permanently remove the repository from the organization. This action is irreversible.
  - Archive: Lock the repository to prevent further changes while preserving its contents for reference.
  - Deprecate: Mark the repository as deprecated, update the README to reflect its status, and optionally link to a successor repository if applicable.
- Repository name
- Repository admin's name, official email, GitHub username and supervisor's email
- Reason for deletion, archival, or deprecation

All requests will be reviewed by the `AAFC-Bioinfo-AAC` admin team. For deletion, confirmation will be required from both the repository admin and supervisor. Archival and deprecation actions will be completed following internal review and notification.

---

### 2. Account Management

#### 2.1. Add New User

To onboard a new contributor to `AAFC-Bioinfo-AAC`, click **Add new user** and provide:

- User’s name, official email, GitHub username, and supervisor’s email
- Name of repository (one or more) to be added to and role (admin, maintain, write, or read; refer [role permissions guide](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#permissions-for-each-role))

Once approved, the user will be added to the organization and will be assigned roles in repositories requested.

#### 2.2. Remove User

To remove a user from the organization or one or more repositories, click **Remove user** and submit all info as requested in the section 2.1 above, and additionally, the reason for removal.

The request will be reviewed and processed by the admin team. A confirmation will be sent to the repository admin and supervisor.

#### 2.3. Modify User Privileges

To change a user’s role within a repository, click **Modify user privileges** and provide all info as requested in the section 2.1 above.

Role changes will be reviewed to ensure alignment with organizational policies.

---

### 3. Training

Training sessions and onboarding materials are available to help users effectively manage repositories and contribute to projects. These include:

- Introductory GitHub tutorials for new users
- Best practices for collaborative coding and version control
- Guidelines for repository setup, documentation, and publication
- Security and compliance training for open-source contributions

To request training or access materials, contact the `AAFC-Bioinfo-AAC` admin team via this selection.

---

### 4. Other

For any requests not covered by the above categories—such as:

- Repository migration support
- Custom automation or CI/CD setup
- Integration with external tools or platforms
- Technical troubleshooting

Please submit a request here with a clear description of your needs. The support team will assess and follow up accordingly.

---

## Credits

This guide was developed by the **ABCC project team**.

🤖 This project includes content generated with the assistance of AI models. All AI-generated material has been reviewed, verified, and, where necessary, refined by the project team to ensure accuracy.

---

## Citation

To cite this project, click the **`Cite this repository`** button on the right-hand sidebar.

---

## Contribution

Contributions are welcome! Please review the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md) and ensure you adhere to our [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) to foster a respectful and inclusive environment.

---

## Security

⚠️ Do not post any security issues on the public repository! Please report them as described in [SECURITY.md](SECURITY.md).

---

## License

See the [LICENSE](LICENSE) file for details. Visit [LicenseHub](https://licensehub.org) or [tl;drLegal](https://www.tldrlegal.com/) to view a plain-language summary of this license.

**Copyright (c)** His Majesty the King in Right of Canada, as represented by the Minister of Agriculture and Agri-Food, 2025.

---

## Need Help?

Email [BRSN](mailto:aafc.bioinfosupport.aac@agr.gc.ca) with subject: `AAFC-Bioinfo-AAC: <summary>`
