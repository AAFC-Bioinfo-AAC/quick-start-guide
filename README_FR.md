<!-- omit in toc -->
# Guide de démarrage rapide

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](README_FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](https://github.com/AAFC-Bioinfo-AAC/quick-start-guide)

<!-- omit in toc -->
## À propos

Ce guide décrit les services disponibles et les processus recommandés pour gérer et contribuer aux dépôts de code bio-informatique au sein de l’organisation GitHub **AAFC-Bioinfo-AAC**, associée au projet de Codes Bioinformatique d'AAC (RCBA).

<!-- omit in toc -->
## Table des matières

- [Services GitHub *AAFC-Bioinfo-AAC*](#services-github-aafc-bioinfo-aac)
  - [1. Gestion du dépôt](#1-gestion-du-dépôt)
    - [1.1. Créer des dépôts privés](#11-créer-des-dépôts-privés)
    - [1.2. Publier un dépôt (rendre public)](#12-publier-un-dépôt-rendre-public)
    - [1.3. Supprimer / Archiver / Déprécier un dépôt](#13-supprimer--archiver--déprécier-un-dépôt)
  - [2. Gestion des comptes](#2-gestion-des-comptes)
    - [2.1. Ajout de nouveaux utilisateurs](#21-ajout-de-nouveaux-utilisateurs)
    - [2.2. Suppression d'utilisateurs](#22-suppression-dutilisateurs)
    - [2.3. Modification des privilèges de l'utilisateur](#23-modification-des-privilèges-de-lutilisateur)
  - [3. Formation](#3-formation)
  - [4. Autre](#4-autre)
- [Crédits](#crédits)
- [Citation](#citation)
- [Contribution](#contribution)
- [Sécurité](#sécurité)
- [Licence](#licence)
- [Besoin d’aide?](#besoin-daide)

---

## Services GitHub *AAFC-Bioinfo-AAC*

Les services suivants sont disponibles via `Mon IT Centre TI` sous la catégorie : `Support informatique scientifique > AAFC Bioinformatics Code Catalogue` ([lien d’accès interne](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=)).

### 1. Gestion du dépôt

#### 1.1. Créer des dépôts privés

Pour démarrer un nouveau projet ou migrer un projet existant vers l’organisation GitHub `AAFC-Bioinfo-AAC`, cliquez sur **Créer des dépôts privés** et remplissez le formulaire avec :

- Un nom du dépôt conforme aux [conventions de nommage des dépôts AAFC-Bioinfo-AAC](./docs/repo-naming-style-guide.md).
- Une brève description bilingue (anglais et français)
- Le nom de l’administrateur ou de l’administratrice du dépôt, son courriel officiel, son nom d’utilisateur GitHub, ainsi que le courriel du superviseur
- Le cas échéant, la liste des autres utilisateurs de l’équipe avec leurs noms, courriels, noms d’utilisateur GitHub et rôles (administration, gestion, écriture ou lecture ; voir le [guide des permissions par rôle](https://docs.github.com/fr/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization))

Remarques importantes :

- Au moins une personne doit se voir attribuer le rôle d’administrateur.
- L’administrateur est responsable de la maintenance continue du dépôt et de la gestion des utilisateurs.
- Les contributeurs et contributrices doivent suivre les [bonnes pratiques de codage](./docs/coding-best-practices.md#bonnes-pratiques-de-codage--référence-rapide).
- Des utilisateurs additionnels peuvent être ajoutés plus tard par l’administrateur. Si une personne n’est pas encore membre de l’organisation, utilisez le formulaire [Ajouter un nouvel utilisateur](./README_FR.md#21-Ajout-de-nouveaux-utilisateurs) pour assurer un embarquement approprié.

Une fois la demande approuvée, le dépôt sera initialisé à partir du modèle standard, comprenant :

- Des modèles de README bilingues avec conseils et exemples
- La licence MIT avec droit d’auteur de la Couronne
- Des documents standards : `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`, etc.

#### 1.2. Publier un dépôt (rendre public)

Pour demander qu’un dépôt devienne public, cliquez sur **Publier un dépôt** et fournissez :

- Le nom du dépôt
- Le nom de l’administrateur du dépôt, son courriel officiel, son nom d’utilisateur GitHub et le courriel de la personne superviseure
- Un **Formulaire d’approbation pour le développement ou la publication de source ouverte** (lien fourni dans le billet), signé par le directeur de votre Centre  
  *(Téléchargez le formulaire en format Word à partir du lien fourni dans le billet)*

Après un examen de sécurité réussi et l’approbation du directeur de l’ISB, le dépôt sera publié.

#### 1.3. Supprimer / Archiver / Déprécier un dépôt

Pour modifier l’état d’un dépôt, cliquez sur **Supprimer/Archiver/Déprécier un dépôt** et soumettez les éléments suivants :

- Action souhaitée :
  - Supprimer : retirer définitivement le dépôt de l’organisation. Cette action est irréversible.
  - Archiver : verrouiller le dépôt pour empêcher toute modification tout en préservant son contenu à des fins de référence.
  - Déprécier : marquer le dépôt comme déprécié, mettre à jour le README pour refléter ce statut et, au besoin, lier à un dépôt successeur.
- Nom du dépôt
- Nom de l’administrateur du dépôt, son courriel officiel, son nom d’utilisateur GitHub et le courriel du superviseur
- Raison de la suppression, de l’archivage ou de la dépréciation

Toutes les demandes seront examinées par l’équipe d’administration `AAFC-Bioinfo-AAC`. Pour une suppression, une confirmation sera requise de la part de l’administrateur du dépôt **et** du superviseur. Les actions d’archivage et de dépréciation seront effectuées à la suite d’un examen interne et d’une notification.

---

### 2. Gestion des comptes

#### 2.1. Ajout de nouveaux utilisateurs

Pour intégrer un nouveau contributeur à `AAFC-Bioinfo-AAC`, cliquez sur **Ajout de nouveaux utilisateurs** et fournissez :

- Le nom de l'utilisateur, son courriel officiel, son nom d’utilisateur GitHub et le courriel du superviseur
- Le nom du dépôt auquel l’ajouter et le rôle souhaité (administrateur, gestion, écriture ou lecture; voir le [guide des permissions par rôle](https://docs.github.com/fr/organizations/managing-user-access-to-your-organizations-repositories/managing-repository-roles/repository-roles-for-an-organization#permissions-for-each-role))

Une fois approuvée, la personne sera ajoutée à l’organisation et se verra attribuer les rôles demandés dans les dépôts concernés.

#### 2.2. Suppression d'utilisateurs

Pour retirer une personne de l’organisation ou d’un ou plusieurs dépôts, cliquez sur **Suppression d'utilisateurs** et fournissez toutes les informations demandées à la section 2.1 ci‑dessus, ainsi que la raison du retrait.

La demande sera examinée et traitée par l’équipe d’administration. Une confirmation sera envoyée à l’administrateur du dépôt et au superviseur.

#### 2.3. Modification des privilèges de l'utilisateur

Pour modifier le rôle d’une personne dans un dépôt, cliquez sur **Modification des privilèges de l'utilisateur** et fournissez toutes les informations demandées à la section 2.1 ci‑dessus.

Les changements de rôle seront examinés afin d’assurer leur conformité aux politiques de l’organisation.

---

### 3. Formation

Des séances de formation et du matériel d’intégration sont offerts pour aider les utilisateurs et utilisatrices à gérer efficacement les dépôts et à contribuer aux projets. Ceux‑ci incluent :

- Tutoriels GitHub d’introduction pour les nouveaux utilisateurs
- Bonnes pratiques pour la collaboration et le contrôle de version
- Lignes directrices pour la configuration, la documentation et la publication d’un dépôt
- Formation sur la sécurité et la conformité pour les contributions au code source ouvert

Pour demander une formation ou accéder au matériel, communiquez avec l’équipe d’administration `AAFC-Bioinfo-AAC` au moyen de cette option.

---

### 4. Autre

Pour toute demande qui n’est pas couverte par les catégories ci‑dessus — par exemple :

- Soutien à la migration de dépôts
- Automatisation personnalisée ou configuration CI/CD
- Intégration avec des outils ou plateformes externes
- Dépannage technique

Veuillez soumettre ici une demande en décrivant clairement vos besoins. L’équipe de soutien évaluera la demande et assurera le suivi en conséquence.

---

## Crédits

Ce guide a été élaboré par l’**équipe du projet ABCC**.

🤖 Ce projet inclut du contenu généré avec l’aide de modèles d’IA. Tout le matériel généré par IA a été examiné, vérifié et, au besoin, affiné par l’équipe du projet afin d’en assurer l’exactitude.

---

## Citation

Pour citer ce projet, cliquez sur le bouton **`Cite this repository`** dans la barre latérale de droite.

---

## Contribution

Les contributions sont les bienvenues ! Veuillez consulter les lignes directrices dans [CONTRIBUTING.md](CONTRIBUTING.md) et vous assurer de respecter notre [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) afin de favoriser un environnement respectueux et inclusif.

---

## Sécurité

⚠️ Ne publiez aucun problème de sécurité sur le dépôt public! Veuillez le signaler comme décrit dans [SECURITY.md](SECURITY.md).

---

## Licence

Voir le fichier [LICENSE](LICENSE) pour plus de détails. Visitez [LicenseHub](https://licensehub.org/fr) ou [tl;drLegal](https://www.tldrlegal.com/) pour consulter un résumé en langage clair de cette licence.

**Droit d’auteur (c)** Sa Majesté le Roi du chef du Canada, représenté par le ministre de l’Agriculture et de l’Agroalimentaire, 2025.

---

## Besoin d’aide?

Écrivez à [BRSN](mailto:aafc.bioinfosupport.aac@agr.gc.ca) avec l’objet : `AAFC-Bioinfo-AAC: <summary>`
