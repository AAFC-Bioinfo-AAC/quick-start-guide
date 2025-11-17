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
    - [Avant la publication](#avant-la-publication)
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

- Installation de Git: faire une demande dans [*Mon Centre TI → Demandes d'autres logiciels*]().
- Compte GitHub: si vous n'en avez pas déjà un, [créez-en un](https://github.com/signup).
- [Authentification GitHub](https://docs.github.com/en/authentication): nécessaire pour toute interaction autre que l'interface Web.

> [!TIP]
> Si votre compte GitHub est principalement utilisé pour des projets personnels, envisagez d'en créer un destiné au travail (ex. `prenom-nom-aafc`). Selon le *Guide de publication de code source ouvert*, les employés doivent utiliser leur nom complet et leur adresse courriel du gouvernement du Canada pour tout code publié dans le cadre de leurs fonctions.

---

### Devenir membre

Pour rejoindre l'organisation *AAFC‑Bioinfo‑AAC*, soumettez un billet TI via *Mon Centre TI → Soutien TI scientifique → Catalogue de code bioinformatique d'AAC → Gestion des comptes → Ajouter un nouvel utilisateur*.

Fournissez les renseignements requis, notamment votre nom d'utilisateur GitHub et les dépôts auxquels vous avez besoin d'accéder. Une invitation vous sera envoyée une fois la demande approuvée.

---

### Créer un nouveau dépôt GitHub

Pour démarrer un nouveau projet, soumettez un billet TI via *Mon Centre TI → Soutien TI scientifique → Catalogue de code bioinformatique d'AAC → Gestion des dépôts → Créer un nouveau dépôt privé*.

Indiquez les renseignements requis, y compris le nom du dépôt (voir les conventions de nommage) et l'administrateur responsable. Le dépôt sera créé à partir du modèle standard *AAFC‑Bioinfo‑AAC*, que vous pouvez modifier au besoin tout en conservant les sections obligatoires.

L'administrateur du dépôt peut ajouter directement des utilisateurs. Toutefois, s'il s'agit d'employés d'AAC ne faisant pas encore partie de l'organisation, il est préférable qu'ils en deviennent membres avant leur ajout.

---

### Migrer un dépôt existant

Créez un nouveau dépôt selon le processus ci‑dessus, puis migrez-y votre projet vous‑même ou en soumettant un billet TI (option : Autre).

---

### Développer le projet

- Clonez le dépôt GitHub sur votre ordinateur et appliquez les pratiques Git standard : *pull → branche → modification → commit → push → PR → révision → fusion → mise à jour → répétition*.
- Suivez les bonnes pratiques de développement.
- Ne poussez jamais de données sensibles, confidentielles ou protégées. Configurez adéquatement votre `.gitignore`.

> \[!IMPORTANT\]\
> Ne clonez jamais un dépôt dans un dossier synchronisé (OneDrive, Google Drive, Dropbox, etc.). Cela peut entraîner des corruptions de fichiers et des erreurs de performance.

---

### Publier un projet

Lorsque votre projet est prêt à devenir public, soumettez une demande via *Mon Centre TI → Soutien TI scientifique → Catalogue de code bioinformatique d'AAC → Gestion des dépôts → Publier un dépôt*.

Joignez le formulaire d'approbation interne pour la publication ou le développement de logiciels libres. Le dépôt sera examiné par les équipes de sécurité internes avant d'être rendu public.

#### Avant la publication

- Mettez à jour votre `README.md` et votre documentation.
- Assurez-vous que les fichiers obligatoires provenant du modèle sont remplis:
  - `dockstore.yml`
  - `CITATION.cff`
  - `LICENSE`

#### Après la publication

- Vérifiez qu'aucune information sensible n'est contenue dans le dépôt.
- Ajoutez ou mettez à jour les *topics* GitHub.
- Créez une version officielle (release) au besoin.
  - Maintenez la documentation, les dépendances et la gouvernance du projet.
  - Suivez les statistiques du dépôt.
- Si le projet devient inactif, consultez les lignes directrices pour l'archivage ou la dépréciation.

---

## Ressources d'apprentissage

- Tutoriel Git de W3Schools
- Apprendre Git (git-scm.com)
- Premiers pas avec GitHub

---

## Remerciements

Ce guide a été élaboré par l’équipe du projet `Répertoire de Codes Bioinformatique d'AAC (RCBA)`.

🤖 Ce projet inclut du contenu généré avec l’aide de modèles d’IA. Tout le matériel généré par IA a été examiné, vérifié et, au besoin, affiné par l’équipe du projet afin d’en assurer l’exactitude.

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
