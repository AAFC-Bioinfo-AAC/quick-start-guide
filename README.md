<!-- omit in toc -->
# Quick Start Guide

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](README_FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](https://github.com/AAFC-Bioinfo-AAC/quick-start-guide)

<!-- omit in toc -->
## About

This guide provides a streamlined process for creating, managing, and contributing to bioinformatics code repositories within the **AAFC-Bioinfo-AAC** GitHub organization. It includes repository setup, publishing procedures, and coding best practices, among others.

<!-- omit in toc -->
## Table of Contents

- [Overview](#overview)
  - [*AAFC-Bioinfo-AAC* GitHub services](#aafc-bioinfo-aac-github-services)
    - [1. Repository Management](#1-repository-management)
      - [1.1. Create a new private repository](#11-create-a-new-private-repository)
        - [Pre-requisites](#pre-requisites)
        - [Post-approval](#post-approval)
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

## Overview

### *AAFC-Bioinfo-AAC* GitHub services

The following services are available via `My IT Centre TI` (internal access only) under category: `Science IT Support > AAFC Bioinformatics Code Catalogue`, to support the *AAFC-Bioinfo-AAC* GitHub organization associated with the AAFC Bioinformatics Code Catalogue project (ABCC).

---

#### 1. Repository Management

##### 1.1. Create a new private repository

Complete and submit the **Create a new private repository** form to request a new repository on *AAFC-Bioinfo-AAC*, either to develop a fresh project or to [migrate an existing repository](./README.md#migrating-an-existing-repository) from another location to continue development here.

###### Pre-requisites

Prior to submitting the ticket, ensure that you have the following information ready:

- A repository name that complies with the [AAFC-Bioinfo-AAC repository naming conventions](./docs/repo-naming-style-guide.md).
- A concise, one-line description of the repository in both English and French.
- A list of GitHub usernames and roles (`admin`, `maintain`, `read` or `write`; refer [permissions-for-each-role](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#permissions-for-each-role)) of all members to be added to the repo.
  - At least one user must be assigned the `admin` role.
  - Additional members may be added later directly by the `admin`. However, if a user is not yet part of `AAFC-Bioinfo-AAC`, the recommended method is to use the [Add new user](./README.md#21-add-new-user) form, to manage organizational membership consistently.

###### Post-approval

Once the ticket is approved, the designated repository `admin` will be notified by email of the new repository, initialized from the `AAFC-Bioinfo-AAC` template repository, with the following content included:

- English and French `README` templates (with instructions for recommended sections and example content).
- A default MIT License with Crown copyright.
- Standard supporting documents (e.g., `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, etc.).

The repository `admin` is responsible for ongoing maintenance, ensuring that the team members and roles are properly managed. All contributors are expected to apply established [coding best practices](./docs/coding-best-practices.md).

##### 1.2. Publish a repository

To make a repository public:

1. Ensure:
   - All steps in the Approval Process for Open Source Code have been completed (link provided in ticket)
   - The required form and checklist are completed (link provided in ticket).
   - The license is correctly set (consult OIPC/Commercialization Officer if uncertain).

2. Submit a ticket via *MyITCentreTI*:

   ```text
   Science IT Support > Science Code Catalogue > Repository Management > Reviewing repositories for approval before publication
   ```

##### 1.3. Delete/Archive/Deprecate repository

---

#### 2. Account Management

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

##### 2.1. Add new user

##### 2.2. Remove user

##### 2.3. Modify user privileges

---

#### 3. Training

---

#### 4. Other

---

### Migrating an Existing Repository

To migrate an external GitHub repository into the AAFC organization:

- Clone or back up your existing repository
- Follow the standard request process to [create a new repository](#requesting-a-new-github-repository)
- Push your local code to the new repository

---

### Contributing to Existing Repositories

#### Public Repositories

- Open Github issues to suggest features, report bugs, or initiate discussions.
- Fork the repository, make edits and open a pull request per `CONTRIBUTING.md` guidelines.

#### Private Repositories

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
