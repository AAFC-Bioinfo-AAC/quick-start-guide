# Guide de démarrage rapide

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](README_FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](https://github.com/AAFC-Bioinfo-AAC/quick-start-guide)

## À propos

Ce guide propose un processus simplifié pour la création, la gestion et la contribution aux dépôts de code bio-informatique au sein de l’organisation GitHub **AAFC-Bioinfo-AAC**. Il inclut les étapes de configuration des dépôts, de publication ainsi que les meilleures pratiques de contribution.

## Table des matières

- [Guide de démarrage rapide](#guide-de-démarrage-rapide)
  - [À propos](#à-propos)
  - [Table des matières](#table-des-matières)
  - [Aperçu](#aperçu)
    - [Faire une demande d'un nouveau dépôt GitHub](#faire-une-demande-dun-nouveau-dépôt-github)
    - [Publication d’un dépôt](#publication-dun-dépôt)
    - [Migration d’un dépôt existant](#migration-dun-dépôt-existant)
    - [Gestion de l’accès d'un dépôt](#gestion-de-laccès-dun-dépôt)
    - [Contributions aux dépôts existants](#contributions-aux-dépôts-existants)
      - [Dépôts publics](#dépôts-publics)
      - [Dépôts privés](#dépôts-privés)
  - [Crédits](#crédits)
  - [Contribution](#contribution)
  - [Licence](#licence)
  - [Besoin d’aide?](#besoin-daide)

---

## Aperçu

### Faire une demande d'un nouveau dépôt GitHub

Pour faire une demande d'un nouveau dépôt:

1. Soumettre un billet via MyITCentreTI:
   
  ```
  Science TI Support > Catalogue du code scientifique > Gestion de dépôt > Création de dépôts privés
  ```

2. Inclure les informations suivantes:
  - Nom d’utilisateur GitHub de l’administrateur du dépôt
  - Courriel du superviseur de l’administrateur
  - Nom proposé pour le dépôt (suivre le [Guide pour nommer un dépôt](/docs/repo-naming-style-guide.md/))
  - Brève description bilingue (1 à 2 lignes, EN/FR)

Un membre de l’équipe communiquera avec l’administrateur du dépôt sous peu avec un lien vers le nouveau dépôt, initialisé à partir du [dépôt de gabarit](https://github.com/AAFC-Bioinfo-AAC/template-repository), qui comprend:
   - Un modèle `README.md` avec sections recommandées et exemple de contenu
   - Une licence (MIT) avec droits d’auteur de la Couronne
   - Des documents de soutien (ex. `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `SECURITY.md`)

Plus de détails sont fournis dans le [Guide d'utilisateur du dépôt de gabarit](docs/template-repo-user-guide.md).

L’administrateur désigné (demandeur du billet ou membre de l’équipe) est responsable de la maintenance du dépôt, en veillant à:
- Gérer adéquatement les membres et leurs rôles
- S’assurer que le dépôt est facile à reproduire, documenté de façon claire, et simple à comprendre et utiliser.

---

### Publication d’un dépôt

Pour rendre un dépôt public:

1. S’assurer que:
    - Toutes les étapes du Processus d’approbation pour le développement de code source ouvert sont complétées (lien fourni dans le billet)
    - Le formulaire requis et la liste de vérification sont remplis (lien fourni dans le billet)
    - La licence est correctement définie (consulter l’agent de commercialisation si incertain)

2. Soumettre un billet via Mon ITCentreTI:**  
  ```
  Support informatique scientifique > Science Code Catalogue > Gestion de dépôt > Examen des repo pour approbation avant publication
  ```

---

### Migration d’un dépôt existant

Pour migrer un dépôt GitHub externe vers l’organisation AAC:

- Cloner ou sauvegarder votre dépôt existant
- Suivre le processus standard de demande pour [créer un nouveau dépôt](#faire-une-demande-dun-nouveau-dépôt-github)
- Pousser votre code local vers le nouveau dépôt

---

### Gestion de l’accès d'un dépôt

- Les administrateurs d'un dépôt peuvent eux-mêmes ajouter des membres et attribuer des rôles.
- Pour modifier l’accès ou les rôles, soumettre un billet via MyITCentreTI:  

  ```
  Science TI Support > Catalogue du code scientifique > Gestion des comptes
  ```

- **Seuls les propriétaires de l’organisation GitHub d'AAC** peuvent créer et supprimer des dépôts ou changer les paramètres globaux.

- Pour demander la suppression, l’archivage ou la dépréciation d’un dépôt, soumettre un billet à Mon ITCentreTI:  
  
  ```
  Support informatique scientifique > Science Code Catalogue > Gestion de dépôt
  ```

---

### Contributions aux dépôts existants

#### Dépôts publics

- Utiliser la fonction *Issues* de GitHub pour suggérer des fonctionnalités, signaler des bogues ou entamer des discussions.
- Dupliquer (*fork*) le dépôt, apporter des modifications puis utiliser la fonction *Pull requests* selon les directives de `CONTRIBUTING.md`.

#### Dépôts privés

- Se référer à la liste interne des [Dépôts de code privés](https://001gc.sharepoint.com/:u:/r/sites/42732/SitePages/abcc-private-repos.aspx?csf=1&web=1&e=jXxrXb).
- Contacter le propriétaire/gestionnaire du dépôt pour un accès ou une collaboration.

---

## Crédits

Développé et maintenu par l’équipe ABCC.

Ce projet contient du contenu partiellement généré par des modèles d’IA. Tout le matériel généré par IA a été révisé et validé pour l’exactitude par l’équipe du projet.

---

## Contribution

Si vous souhaitez contribuer à ce projet, veuillez consulter les directives dans [CONTRIBUTING.md](CONTRIBUTING.md) et vous assurer de respecter notre [Code de conduite](CODE_OF_CONDUCT.md) afin de promouvoir un environnement respectueux et inclusif.

---

## Licence

Ce projet est distribué sous la licence MIT. Pour les détails complets et droits d’auteur, voir le fichier [LICENSE](LICENSE).


---

## Besoin d’aide?

Pour un soutien général, veuillez envoyer un courriel au [Réseau de soutien à la recherche en bio-informatique](mailto:aafc.bioinfosupport.aac@agr.gc.ca), en utilisant un objet commençant par "ABCC:" suivi d’un bref résumé de votre problème.

🚫 **Ne divulguez pas publiquement les problèmes de sécurité.**  
Pour signaler une vulnérabilité, écrivez à l’équipe de soutien [BICoE](mailto:aafc.bice-ceib.aac@agr.gc.ca).
