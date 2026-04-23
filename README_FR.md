<!-- omit in toc -->
# Guide de démarrage rapide

[![FR](https://img.shields.io/badge/lang-FR-yellow.svg)](README_FR.md)
[![EN](https://img.shields.io/badge/lang-EN-blue.svg)](README.md)

---
<!-- omit in toc -->
## Table of Contents

- [À propos](#à-propos)
- [Pour commencer](#pour-commencer)
  - [Prérequis](#prérequis)
  - [Devenir membre](#devenir-membre)
  - [Créer un nouveau dépôt GitHub](#créer-un-nouveau-dépôt-github)
  - [Migrer un dépôt existant](#migrer-un-dépôt-existant)
  - [Développer le projet](#développer-le-projet)
  - [Publier un projet](#publier-un-projet)
    - [Avant de demander la publication](#avant-de-demander-la-publication)
      - [Instructions pour remplir le formulaire](#instructions-pour-remplir-le-formulaire)
    - [Demander la publication](#demander-la-publication)
    - [Après la publication](#après-la-publication)
- [Ressources d'apprentissage](#ressources-dapprentissage)
- [Remerciements](#remerciements)
- [Contribution](#contribution)
- [Sécurité](#sécurité)
- [Licence](#licence)
- [Besoin d’aide?](#besoin-daide)

---

## À propos

Ce dépôt sert de référence d'accueil pour les nouveaux et actuels membres de l'organisation GitHub *AAFC‑Bioinfo‑AAC*.

L'adhésion et l'accès aux services sont réservés aux employés d'AAC ainsi qu'aux collaborateurs externes approuvés par l'intermédiaire du partenaire d'AAC.

Les demandes de service et les notifications connexes sont gérées par le système interne de billetterie TI d'AAC, accessible via [*Mon Centre TI → Soutien TI scientifique → Catalogue de code bioinformatique d'AAC*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Des indications sur les renseignements requis pour chaque type de demande se trouvent dans le [Guide des services GitHub d'AAFC‑Bioinfo‑AAC](./docs/aafc-bioinfo-aac-github-services-FR.md).

---

## Pour commencer

### Prérequis

- Installation de Git: faire une demande dans [*Mon Centre TI → Demande d'autre logiciel*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHUYTCMJTEZRW63TUMV4HIVDZOBST2Q2BKRAUYT2HL5EE6TKF).
- Compte GitHub: si vous n'en avez pas déjà un, [créez-en un](https://github.com/signup).
- [Authentification GitHub](https://docs.github.com/fr/authentication): nécessaire pour toute interaction autre que l'interface Web.

> [!TIP]
> Si votre compte GitHub est principalement utilisé pour des projets personnels, envisagez d'en créer un destiné au travail (ex. `prenom-nom-aafc`). Selon le [*Guide pour la publication du code source libre*](https://www.canada.ca/fr/gouvernement/systeme/gouvernement-numerique/innovations-gouvernementales-numeriques/logiciels-libres/guide-pour-la-publication-du-code-source-libre.html#:~:text=S%E2%80%99identifier%20en%20tant%20qu%E2%80%99employ%C3%A9%20du%20gouvernement%20du%20Canada), les employés doivent utiliser leur nom complet et leur adresse courriel du gouvernement du Canada pour tout code publié dans le cadre de leurs fonctions.

---

### Devenir membre

Pour rejoindre l'organisation *AAFC‑Bioinfo‑AAC*, soumettez un billet TI via [*Mon Centre TI → Support informatique scientifique → AAFC Bioinformatics Code Catalogue (ABCC) → Gestion des comptes → Ajouter de nouveaux utilisateurs*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Fournissez les [renseignements requis](./docs/aafc-bioinfo-aac-github-services-FR.md#ajout-de-nouveaux-utilisateurs), notamment votre nom d'utilisateur GitHub et les dépôts auxquels vous avez besoin d'accéder. Une invitation vous sera envoyée une fois la demande approuvée.

---

### Créer un nouveau dépôt GitHub

Pour démarrer un nouveau projet, soumettez un billet TI via [*Mon Centre TI → Support informatique scientifique → AAFC Bioinformatics Code Catalogue (ABCC) → Gestion des dépôts → Créer un nouveau dépôt privé*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

Indiquez les [renseignements requis](./docs/aafc-bioinfo-aac-github-services-FR.md#ajout-de-nouveaux-utilisateurs), y compris le nom du dépôt ([voir les conventions de nommage](./docs/repo-naming-style-guide.md)) et l'administrateur responsable. Le dépôt sera créé à partir du [modèle standard *AAFC‑Bioinfo‑AAC*](https://github.com/AAFC-Bioinfo-AAC/template-repository/blob/main/README_FR.md), que vous pouvez modifier au besoin tout en conservant les sections obligatoires.

L'administrateur du dépôt peut ajouter directement des utilisateurs. Toutefois, s'il s'agit d'employés d'AAC ne faisant pas encore partie de l'organisation, il est préférable qu'ils en deviennent membres avant leur ajout.

---

### Migrer un dépôt existant

Créez un nouveau dépôt selon le processus ci‑dessus, puis migrez-y votre projet vous‑même ou en soumettant un billet TI: [*Mon Centre TI → Support informatique scientifique → AAFC Bioinformatics Code Catalogue (ABCC) → Autre*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

---

### Développer le projet

- Clonez le dépôt GitHub sur votre ordinateur et appliquez les pratiques Git standard : *Pull → Branch → Change → Commit → Push → PR → Review → Merge → Update → Repeat*

- Suivez les [bonnes pratiques de développement](./docs/coding-best-practices.md).

- Ne poussez jamais de données sensibles, confidentielles ou protégées. Configurez adéquatement votre `.gitignore`.

> [!IMPORTANT]
> **Ne clonez pas** et ne stockez pas votre copie de travail dans un dossier synchronisé par un service de stockage infonuagique (p. ex., OneDrive, Dropbox, Google Drive, iCloud, etc.). Pour éviter la corruption de fichiers et les problèmes de performance, conservez toujours vos dépôts dans un emplacement non synchronisé — par exemple, un dossier local sous `C:\Users\<nom_utilisateur>` ou dans WSL (`/home/<nom_utilisateur>`).

---

### Publier un projet

#### Avant de demander la publication

- Passez en revue et mettez à jour votre fichier `README.md` ainsi que la documentation du projet afin de vous assurer qu’ils reflètent fidèlement l’état actuel et l’objectif de votre projet.
- Assurez-vous que les fichiers suivants (provenant du modèle standard [*AAFC-Bioinfo-AAC*](https://github.com/AAFC-Bioinfo-AAC/template-repository/blob/main/README_FR.md)) sont complétés ou adaptés à votre projet, en suivant les instructions fournies dans ces fichiers ou dans la section correspondante du README du modèle :
  - `LICENSE`: La licence par défaut est **MIT** — remplacez-la si nécessaire. Un outil interne R Shiny, [*OSSLicensR*](https://websphn001.agr.gc.ca/OSSLicensR/) (accès interne uniquement), est disponible pour vous aider à sélectionner une licence appropriée.
  - `CITATION.cff`: Fournis les métadonnées de citation afin d’encourager l’attribution appropriée de votre logiciel ou flux de travail lorsqu’il est réutilisé par d’autres.
  - `dockstore.yml`: Fournis les métadonnées nécessaires pour publier des flux de travail analytiques sur [Dockstore](https://dockstore.org/) — une plateforme de partage d’outils et de pipelines développés avec CWL, WDL, Nextflow, Snakemake ou Galaxy. ***Supprimez ce fichier si la publication sur Dockstore ne s’applique pas à votre projet.***

- Remplissez le *Formulaire d’approbation pour le développement ou la publication de code source ouvert* (voir [Instructions pour remplir le formulaire](#instructions-pour-remplir-le-formulaire)).

##### Instructions pour remplir le formulaire

Le responsable du projet/dépôt doit remplir les sections A et B du Formulaire d’approbation pour le développement ou la publication de code source ouvert ([lien interne](https://001gc.sharepoint.com/sites/34851/asd1/A9702-F.pdf)) et le faire signer par le directeur délégué de son centre.

#### Demander la publication

Lorsque votre projet est prêt à devenir public, soumettez une demande via [*Mon Centre TI → Support informatique scientifique → AAFC Bioinformatics Code Catalogue (ABCC) → Gestion des dépôts → Publier un dépôt*](https://aafcaac-dwp.ca.onbmc.com/dwp/rest/share/OJSXG33VOJRWKVDZOBST2U2CL5IVKRKTKREU6TSOIFEVERJGORSW4YLOOREWIPKBI5DUKWKKHA4EUNKUJBBUCU2KJNAVASSTJJFUCUCKJM4TKWRGOJSXG33VOJRWKSLEHU2TANJGMNXW45DFPB2FI6LQMU6UGQKUIFGE6R27JBHU2RI=).

[Fournissez les renseignements requis](./docs/aafc-bioinfo-aac-github-services-FR.md#publier-un-dépôt-rendre-public) et joignez le *Formulaire d’approbation pour le développement ou la publication de code source ouvert* dûment rempli (voir [Instructions pour remplir le formulaire](#instructions-pour-remplir-le-formulaire)).

Après un examen de sécurité réussi et l’approbation du directeur de l’ISB, le dépôt sera publié.

#### Après la publication

- L’URL du dépôt devient accessible publiquement; vérifiez de nouveau qu’aucune information sensible ou donnée interne n’est exposée avant d’annoncer ou de partager le lien.
- Ajoutez ou mettez à jour les [rubriques et mots-clés GitHub](https://docs.github.com/fr/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/classifying-your-repository-with-topics) afin d’améliorer la découvrabilité.
- Si le projet comprend une application ou un composant distribuable, créez une version officielle (*release*).
  - Identifiez chaque version à l’aide du schéma de [Gestion sémantique de version](https://semver.org/lang/fr/) (p. ex., `v1.0.0`) afin de communiquer clairement les changements et de maintenir un historique prévisible des versions.
  - Fournissez éventuellement des notes de version résumant les principaux changements, correctifs ou nouvelles fonctionnalités pour aider les utilisateurs à comprendre ce que contient chaque version.
- Maintenez à jour les métadonnées, la documentation et les dépendances.
- Poursuivez la gouvernance : gérez les *issues* et *pull requests* conformément aux normes de contribution `AAFC-Bioinfo-AAC`.
- Surveillez les statistiques du dépôt (trafic, *forks*, citations) pour mesurer l’engagement et planifier les améliorations.
- Si le dépôt devient inactif, suivez les directives du cycle de vie des dépôts pour [l’archivage ou la dépréciation](./docs/aafc-bioinfo-aac-github-services-FR.md#supprimer--archiver--déprécier-un-dépôt).

---

## Ressources d'apprentissage

- [Tutoriel Git de W3Schools](https://www.w3schools.com/git/default.asp)
- [Apprendre Git](https://git-scm.com/learn)
- [Bien démarrer avec la documentation GitHub](https://docs.github.com/fr/get-started)

---

## Remerciements

Ce guide a été élaboré par l’équipe du projet `Répertoire de Codes Bioinformatique d'AAC (RCBA)`.

🤖 Ce projet inclut du contenu généré avec l’aide de modèles d’IA. Tout le matériel généré par IA a été examiné, vérifié et, au besoin, affiné par l’équipe du projet afin d’en assurer l’exactitude.

---

## Contribution

Les contributions sont les bienvenues! Veuillez consulter les lignes directrices dans [CONTRIBUTING.md](CONTRIBUTING.md) et vous assurer de respecter notre [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) afin de favoriser un environnement respectueux et inclusif.

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
