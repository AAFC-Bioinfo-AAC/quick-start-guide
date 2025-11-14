<!-- omit in toc -->
# `AAFC-Bioinfo-AAC` GitHub services

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](../docs/aafc-bioinfo-aac-github-services-FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](../docs/aafc-bioinfo-aac-github-services-EN.md)

<!-- omit in toc -->
## About

This guide describes available services and processes to manage and contribute to bioinformatics code repositories within the **AAFC-Bioinfo-AAC** GitHub organization. These services, categorized under 4 types of requests, are managed through AAFC’s internal IT ticketing system, accessible via [*My IT Centre TI → Science IT Support → AAFC Bioinformatics Code Catalogue*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

<!-- omit in toc -->
## Type of Request

- [Repository Management](#repository-management)
  - [Create a new private repository](#create-a-new-private-repository)
  - [Publish a repository (make Public)](#publish-a-repository-make-public)
  - [Delete/Archive/Deprecate repository](#deletearchivedeprecate-repository)
- [Account Management](#account-management)
  - [Add New User](#add-new-user)
  - [Remove User](#remove-user)
  - [Modify User Privileges](#modify-user-privileges)
- [Training](#training)
- [Other](#other)

---

## Repository Management

### Create a new private repository

To initiate a new project or migrate an existing one to the `AAFC-Bioinfo-AAC` GitHub organization, click **Create a new private repository** and complete the form with:

- A repository name following [AAFC-Bioinfo-AAC repository naming conventions](../docs/repo-naming-style-guide.md).
- A brief bilingual description (English and French)
- Repository admin’s name, official email, GitHub username, and supervisor’s email
- If applicable, a list of team members with their names, email, GitHub username and assigned roles (admin, maintain, write, or read; refer [role permissions guide](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#permissions-for-each-role))

Important Notes:

- At least one user must be assigned the admin role.
- The admin is responsible for ongoing repository maintenance and user management.
- Contributors must follow [coding best practices](../docs/coding-best-practices.md).
- Additional users can be added later by the admin. If a user is not yet part of the organization, use the [Add new user](./aafc-bioinfo-aac-github-services-EN.md#add-new-user) form to ensure proper onboarding.

Once approved, the repository will be initialized from the standard template, including:

- Bilingual README templates with guidance and examples
- MIT License with Crown copyright
- Standard documents: `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, etc.

### Publish a repository (make Public)

To request that a repository be made public, click **Publish a repository** and provide:

- Repository name
- Repository admin's name, official email, GitHub username and supervisor's email
- A completed **Open-Source Development or Publication Approval Form** signed by the Associate Director of your Centre  
  *(Download the form as a Word document from the link provided in the ticket)*

After a successful security review and ISB Director approval, the repository will be published.

### Delete/Archive/Deprecate repository

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

## Account Management

### Add New User

To join `AAFC-Bioinfo-AAC` as a new member or to be added to an existing repository, click **Add new user** and provide:

- User’s name, official email, GitHub username, and supervisor’s email
- Name of repository (one or more) to be added to and role (admin, maintain, write, or read; refer [role permissions guide](https://docs.github.com/en/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#permissions-for-each-role))
  - For new member requests, indicate "NA" under `The repository name(s)` and `The user's role` fields and "New member" under `Additional Information` field.

Once approved, the user will be added to the organization and will be assigned roles in repositories requested.

### Remove User

To remove a user from the organization or one or more repositories, click **Remove user** and submit all info as requested in the section 2.1 above, and additionally, the reason for removal.

The request will be reviewed and processed by the admin team. A confirmation will be sent to the repository admin and supervisor.

### Modify User Privileges

To change a user’s role within a repository, click **Modify user privileges** and provide all info as requested in the section 2.1 above.

Role changes will be reviewed to ensure alignment with organizational policies.

---

## Training

Training sessions and onboarding materials are available to help users effectively manage repositories and contribute to projects. These include:

- Introductory GitHub tutorials for new users
- Best practices for collaborative coding and version control
- Guidelines for repository setup, documentation, and publication
- Security and compliance training for open-source contributions

To request training or access materials, contact the `AAFC-Bioinfo-AAC` admin team via this selection.

---

## Other

For any requests not covered by the above categories—such as:

- Repository migration support
- Custom automation or CI/CD setup
- Integration with external tools or platforms
- Technical troubleshooting

Please submit a request here with a clear description of your needs. The support team will assess and follow up accordingly.

---
