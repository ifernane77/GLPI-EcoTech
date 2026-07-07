# Journal de bord — GLPI EcoTech

## Semaine 1 — Cadrage initial du projet GLPI

### Objectif de la semaine

L’objectif de cette semaine était de définir le périmètre du projet GLPI EcoTech et de préparer les premières preuves pour l’épreuve E5.

Cette semaine correspond à une phase de préparation : définition du contexte, inventaire prévisionnel du parc informatique et création du backlog.

### Travail réalisé

- Création du dossier projet.
- Création ou préparation du dépôt GitHub.
- Rédaction du périmètre du projet.
- Rédaction d’un inventaire prévisionnel du parc informatique.
- Définition des objectifs du projet.
- Création du backlog initial.
- Préparation des premières preuves.

### Difficultés rencontrées

J’ai dû bien distinguer le rôle du projet GLPI par rapport au projet EcoTech Suivi Chantier.

EcoTech Suivi Chantier est une application web liée à l’épreuve E6 SLAM, tandis que GLPI EcoTech est un projet orienté support informatique pour l’épreuve E5.

### Solutions apportées

J’ai séparé les deux projets dans deux dépôts GitHub différents.

J’ai défini GLPI EcoTech comme une simulation professionnelle de gestion du parc informatique, des tickets, des incidents, des demandes internes et d’une base de connaissances.

### Résultat obtenu

Le projet GLPI EcoTech dispose maintenant d’une première base documentaire :

- présentation du projet ;
- périmètre ;
- inventaire prévisionnel ;
- objectifs ;
- backlog ;
- journal de bord.

### Preuves produites

- Capture du dossier local.
- Capture du dépôt GitHub.
- Capture des fichiers Markdown dans VS Code.
- Capture de l’inventaire prévisionnel.
- Capture du backlog.
- Capture du commit Git.

### Lien avec le BTS SIO

Ce projet prépare principalement l’épreuve E5.

Il permet de montrer une démarche de support informatique : gestion du parc, demandes, incidents, documentation et mise à disposition d’un service informatique.

## Semaine 2 — Cartographie du système d’information

### Objectif de la semaine

L’objectif de cette semaine était d’identifier les équipements et les services composant le système d’information d’EcoTech.

Ce travail prépare le projet GLPI EcoTech, qui servira principalement pour l’épreuve E5.

### Travail réalisé

- Recensement du parc cible.
- Création d’une cartographie simple du système d’information.
- Mise à jour de l’inventaire prévisionnel.
- Réflexion sur les règles de sécurisation de base.
- Préparation des éléments à intégrer plus tard dans GLPI.

### Difficultés rencontrées

La difficulté principale a été de rester réaliste et de ne pas imaginer une infrastructure trop complexe par rapport à une petite entreprise.

### Résultat obtenu

Le projet GLPI dispose maintenant d’une première cartographie du système d’information et d’un inventaire plus précis du parc informatique.

Ces documents prépareront l’ajout futur des équipements dans GLPI.

### Preuves produites

- cartographie-si.md
- inventaire-parc.md
- regles-securisation-equipements.md
- capture du schéma Mermaid sur GitHub
- capture du commit Git

## Semaine 3 — Préparation des tickets GLPI

### Objectif de la semaine

L’objectif de cette semaine était de préparer une liste de tickets réalistes à intégrer plus tard dans GLPI.

Ces tickets sont basés sur le contexte de l’entreprise EcoTech et serviront de preuves pour l’épreuve E5.

### Travail réalisé

- Rédaction de 8 tickets réalistes.
- Classification des tickets par type, catégorie et priorité.
- Association des tickets avec des équipements ou services.
- Identification des compétences E5 liées aux tickets.
- Préparation des futures preuves à réaliser dans GLPI.

### Tickets préparés

- PC administratif lent.
- Imprimante / scanner indisponible.
- Demande d’accès à Google Drive.
- Problème d’accès à l’application EcoTech.
- Téléphone professionnel abîmé.
- Devis introuvable.
- Connexion Internet instable via Livebox.
- Mise en place d’une sauvegarde régulière.

### Difficultés rencontrées

La difficulté principale a été de créer des tickets réalistes, adaptés à une petite entreprise, sans inventer une infrastructure trop complexe.

### Résultat obtenu

Le projet GLPI EcoTech dispose maintenant d’une base de tickets qui pourra être saisie plus tard dans GLPI.

Ces tickets permettront de produire des captures et de montrer une démarche professionnelle de support informatique.

### Preuves produites

- tickets-glpi-previsionnels.md
- classification-tickets.md
- capture des tickets dans VS Code
- capture du commit Git

### Lien avec le BTS SIO

Cette semaine est liée à l’épreuve E5, car elle prépare la gestion des incidents, des demandes d’assistance et du patrimoine informatique.

## Semaine 4 — Préparation de l’environnement GLPI

### Objectif de la semaine

L’objectif de cette semaine était de préparer l’environnement technique du projet GLPI EcoTech.

Cette étape prépare l’installation future de GLPI sur une machine virtuelle Debian 11.

### Travail réalisé

- Création du fichier `installation-glpi.md`.
- Création du fichier `environnement-debian.md`.
- Création du fichier `prerequis-glpi.md`.
- Création du fichier `procedure-acces-vm.md`.
- Préparation du dossier de preuves de la semaine 4.
- Mise à jour de la documentation du projet.
- Préparation des captures à réaliser sur la VM Debian.

### Difficultés rencontrées

J’ai compris qu’il ne fallait pas installer GLPI directement sans préparer l’environnement.

Il est important de vérifier d’abord la VM Debian, les prérequis, l’accès réseau et la procédure d’installation.

### Résultat obtenu

Le projet dispose maintenant d’une base documentaire pour préparer l’installation de GLPI.

La VM Debian, les prérequis et la procédure d’accès sont documentés afin de faciliter la suite du projet.

### Preuves produites

- `installation-glpi.md`
- `environnement-debian.md`
- `prerequis-glpi.md`
- `procedure-acces-vm.md`
- capture de l’arborescence VS Code
- capture GitHub
- commit Git

### Lien avec le BTS SIO

Cette semaine est liée à l’épreuve E5 car elle prépare la mise à disposition d’un service informatique, ici GLPI, dans un environnement Debian.

## Semaine 5 — Préparation des catégories GLPI

### Objectif de la semaine

L’objectif de cette semaine était de préparer les catégories qui seront utilisées dans GLPI EcoTech.

Cette étape permet d’organiser les futurs tickets, incidents et demandes avant le paramétrage réel dans GLPI.

### Travail réalisé

- Création du fichier `categories-glpi.md`.
- Préparation des catégories : matériel, impression, réseau, cloud/Google Drive, application EcoTech, documents, sauvegarde et accès utilisateur.
- Création du fichier `correspondance-tickets-categories.md`.
- Association des 8 tickets prévisionnels aux catégories GLPI.
- Création du fichier `plan-parametrage-glpi.md`.
- Préparation des étapes à réaliser plus tard dans GLPI.
- Mise à jour de la documentation du projet.

### Difficultés rencontrées

La difficulté principale a été de garder une organisation simple.

Il aurait été possible de créer beaucoup de catégories, mais j’ai choisi de rester sur des catégories réalistes et adaptées à une petite entreprise comme EcoTech.

### Résultat obtenu

Le projet dispose maintenant d’une structure de catégories GLPI cohérente.

Cette préparation facilitera la création des catégories, des équipements et des tickets lorsque GLPI sera installé.

### Preuves produites

- `categories-glpi.md`
- `correspondance-tickets-categories.md`
- `plan-parametrage-glpi.md`
- capture VS Code
- capture GitHub
- commit Git

### Lien avec le BTS SIO

Cette semaine est liée à l’épreuve E5, car elle prépare l’organisation d’un outil de support informatique, la gestion des incidents, des demandes et du patrimoine informatique.

## Semaine 6 — Schéma du SI EcoTech et flux de support

### Objectif de la semaine

L’objectif de cette semaine était de représenter simplement le système informatique d’EcoTech et les flux de support prévus dans GLPI.

Cette étape permet de comprendre l’environnement avant la saisie des équipements et tickets dans GLPI.

### Travail réalisé

- Création du fichier `schema-si-ecotech.md`.
- Réalisation d’un schéma simple du SI EcoTech.
- Représentation de la Livebox, des postes, des téléphones, de l’imprimante et du serveur GLPI de test.
- Création du fichier `flux-support-glpi.md`.
- Description des flux de support : incident, demande d’accès, problème matériel, problème réseau et demande documentaire.
- Création du fichier `justification-schema-si.md`.
- Justification des choix réalisés pour le schéma.
- Mise à jour de la documentation du projet.

### Difficultés rencontrées

La difficulté principale a été de garder un schéma simple et réaliste.

J’ai évité de représenter une architecture trop complexe afin de rester cohérent avec le contexte d’une petite entreprise.

### Résultat obtenu

Le projet dispose maintenant d’un schéma clair du système informatique EcoTech.

Cette documentation facilitera la future utilisation de GLPI pour gérer le parc informatique, les tickets et les demandes.

### Preuves produites

- `schema-si-ecotech.md`
- `flux-support-glpi.md`
- `justification-schema-si.md`
- capture du schéma Mermaid sur GitHub
- capture VS Code
- capture GitHub
- commit Git

### Lien avec le BTS SIO

Cette semaine est liée à l’épreuve E5, car elle prépare la gestion du patrimoine informatique et le traitement des incidents et demandes dans GLPI.

## Semaine 7 — Préparation des entités, groupes et profils GLPI

### Objectif de la semaine

L’objectif de cette semaine était de préparer les entités, groupes, utilisateurs et profils prévus pour GLPI EcoTech.

Cette étape fait le lien avec les leçons sur les utilisateurs, les groupes et les accès.

### Travail réalisé

- Création du fichier `entites-glpi-prevues.md`.
- Préparation de l’entité principale EcoTech.
- Création du fichier `groupes-utilisateurs-glpi.md`.
- Préparation des groupes : gérants, employés, prestataires, support informatique et administration GLPI.
- Création du fichier `comptes-utilisateurs-prevus.md`.
- Préparation des comptes fictifs à créer plus tard dans GLPI.
- Création du fichier `profils-et-droits-glpi.md`.
- Préparation des profils : demandeur, observateur, technicien et super-admin.
- Création du fichier `preparation-parametrage-utilisateurs.md`.

### Difficultés rencontrées

La difficulté principale a été de ne pas donner trop de droits à tous les utilisateurs.

J’ai donc choisi une organisation simple, avec des groupes et profils adaptés à une petite entreprise.

### Résultat obtenu

Le projet dispose maintenant d’une organisation claire pour les futurs utilisateurs GLPI.

Cette préparation servira lorsque GLPI sera installé et que les comptes pourront être créés réellement.

### Preuves produites

- `entites-glpi-prevues.md`
- `groupes-utilisateurs-glpi.md`
- `comptes-utilisateurs-prevus.md`
- `profils-et-droits-glpi.md`
- `preparation-parametrage-utilisateurs.md`
- capture VS Code
- capture GitHub
- commit Git

### Lien avec le BTS SIO

Cette semaine est liée à l’épreuve E5, car elle prépare l’organisation des utilisateurs, groupes, profils et droits dans un outil de support informatique.