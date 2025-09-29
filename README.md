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
    - [1.2. Publish a repository](#12-publish-a-repository)
    - [1.3. Delete/Archive/Deprecate repository](#13-deletearchivedeprecate-repository)
  - [2. Account Management](#2-account-management)
    - [2.1. Add new user](#21-add-new-user)
    - [2.2. Remove user](#22-remove-user)
    - [2.3. Modify user privileges](#23-modify-user-privileges)
  - [3. Training](#3-training)
  - [4. Other](#4-other)
- [Migrating an Existing Repository](#migrating-an-existing-repository)
- [Contributing to Existing Repositories](#contributing-to-existing-repositories)
  - [Public Repositories](#public-repositories)
  - [Private Repositories](#private-repositories)
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

 [Add new user](./README.md#21-add-new-user) form, to manage organizational membership consistently.

#### 1.2. Publish a repository

To make a repository public, select **Publish a repository** button and complete the form with the following information:

- Repository name
- Repository admin's name, official email address, GitHub username and supervisor's email address
- Attach a completed **Open-Source Development or Publication Approval Form**, signed by the Associate Director of your centre.

Following a successful security review of the repository and ISB Director approval, the repository will be published.

#### 1.3. Delete/Archive/Deprecate repository

To request the removal or status change (Archive/Deprecate) of a repository, select the **Delete/Archive/Deprecate repository** button and complete the form with the following details:

- Repository name
- Repository admin's name, official email address, GitHub username and supervisor's email address
- Reason for deletion, archival, or deprecation
Preferred action:

Delete: Permanently remove the repository from the organization. This action is irreversible.
Archive: Lock the repository to prevent further changes while preserving its contents for reference.
Deprecate: Mark the repository as deprecated, update the README to reflect its status, and optionally link to a successor repository if applicable.

All requests will be reviewed by the `AAFC-Bioinfo-AAC` admin team. For deletion requests, a confirmation will be sent to the repository admin and supervisor before proceeding. Archival and deprecation actions will be completed following internal review and notification.

---

### 2. Account Management

- Repository admins can add team members and assign roles themselves
- For access or role changes, submit a ticket via *MyITCentreTI*:

   ```text
   Science IT Support > Science Code Catalogue > Account Management
   ```

- **Only AAFC GitHub Organization Owners** can create/delete repositories or modify organization-wide settings.

To request repository deletion, archival, or deprecation, submit a *MyITCentreTI* ticket under:

   ```text
   Science IT Support > Science Code Catalogue > Repository Management
   ```

#### 2.1. Add new user

#### 2.2. Remove user

#### 2.3. Modify user privileges

---

### 3. Training

---

### 4. Other

---

## Migrating an Existing Repository

To migrate an external GitHub repository into the AAFC organization:

- Clone or back up your existing repository
- Follow the standard request process to [create a new repository](#requesting-a-new-github-repository)
- Push your local code to the new repository

---

## Contributing to Existing Repositories

### Public Repositories

- Open Github issues to suggest features, report bugs, or initiate discussions.
- Fork the repository, make edits and open a pull request per `CONTRIBUTING.md` guidelines.

### Private Repositories

- Refer to the [internal list of private repositories](https://001gc.sharepoint.com/:u:/r/sites/42732/SitePages/abcc-private-repos.aspx?csf=1&web=1&e=jXxrXb).
- Contact the repository owner/maintainer for access or collaboration.

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
