# Catégories GLPI — GLPI EcoTech

## Objectif

Ce document prépare les catégories qui seront utilisées dans GLPI pour organiser les tickets, les équipements et les demandes internes d’EcoTech.

L’objectif est de faciliter le futur paramétrage de GLPI et de garder une organisation simple, adaptée à une petite entreprise.

---

## Catégories principales prévues

| Catégorie GLPI | Utilisation prévue | Exemple de situation |
|---|---|---|
| Matériel | Problèmes liés aux équipements physiques | PC lent, téléphone abîmé |
| Impression | Problèmes liés à l’imprimante ou au scanner | Imprimante indisponible |
| Réseau | Problèmes de connexion ou d’accès Internet | Livebox instable |
| Cloud / Google Drive | Problèmes liés au stockage en ligne | Accès à un dossier Drive |
| Application EcoTech | Problèmes liés à l’application EcoTech Suivi Chantier | Connexion impossible |
| Documents | Problèmes de recherche ou classement documentaire | Devis introuvable |
| Sauvegarde | Demandes liées à la protection des données | Mettre en place une sauvegarde |
| Accès utilisateur | Création, modification ou réinitialisation d’accès | Mot de passe oublié |

---

## 1. Catégorie Matériel

Cette catégorie regroupe les incidents liés aux équipements physiques.

Exemples :

- ordinateur lent ;
- téléphone professionnel abîmé ;
- poste qui ne démarre plus ;
- matériel à remplacer ;
- équipement à vérifier.

Équipements concernés possibles :

- PC-ADM-01 ;
- PC-ADM-02 ;
- PC-GER-01 ;
- PC-GER-02 ;
- TEL-PRO-01 ;
- TEL-PRO-02 ;
- TEL-PRO-03.

---

## 2. Catégorie Impression

Cette catégorie concerne les problèmes liés à l’imprimante et au scanner.

Exemples :

- imprimante hors ligne ;
- scanner non détecté ;
- file d’attente bloquée ;
- impression impossible ;
- problème de connexion à l’imprimante.

Équipement concerné :

- IMP-SCAN-01.

---

## 3. Catégorie Réseau

Cette catégorie regroupe les problèmes liés à la connexion Internet ou au réseau local.

Exemples :

- connexion Internet instable ;
- Wi-Fi lent ;
- Livebox à redémarrer ;
- accès impossible à Google Drive ;
- coupure réseau.

Équipement concerné :

- BOX-01.

---

## 4. Catégorie Cloud / Google Drive

Cette catégorie concerne les demandes ou incidents liés au stockage en ligne.

Exemples :

- accès à un dossier Google Drive ;
- document non partagé ;
- fichier introuvable dans Drive ;
- problème de droits ;
- classement à revoir.

Service concerné :

- Google Drive.

---

## 5. Catégorie Application EcoTech

Cette catégorie concerne l’application EcoTech Suivi Chantier.

Exemples :

- problème de connexion ;
- accès refusé ;
- rôle utilisateur incorrect ;
- document impossible à ajouter ;
- erreur lors de la consultation d’un chantier.

Service concerné :

- EcoTech Suivi Chantier.

---

## 6. Catégorie Documents

Cette catégorie concerne la recherche, le classement ou la perte de documents.

Exemples :

- devis introuvable ;
- facture mal classée ;
- document PDF non retrouvé ;
- problème de version d’un document ;
- document stocké au mauvais endroit.

Documents concernés :

- devis ;
- factures ;
- plans ;
- documents administratifs ;
- documents de chantier.

---

## 7. Catégorie Sauvegarde

Cette catégorie concerne la protection et la sauvegarde des données importantes.

Exemples :

- mettre en place une sauvegarde ;
- vérifier qu’un dossier est sauvegardé ;
- sauvegarder les photos de chantier ;
- éviter la perte de documents importants.

Données concernées :

- documents PDF ;
- devis ;
- factures ;
- photos de chantier ;
- documents administratifs.

---

## 8. Catégorie Accès utilisateur

Cette catégorie concerne les comptes, mots de passe et droits d’accès.

Exemples :

- mot de passe oublié ;
- création d’un compte ;
- modification d’un rôle ;
- accès refusé à un service ;
- suppression ou désactivation d’un accès.

Services concernés :

- messagerie professionnelle ;
- Google Drive ;
- application EcoTech ;
- poste utilisateur.

---

## Justification

Ces catégories sont simples et adaptées au contexte d’EcoTech.

Elles couvrent les besoins principaux d’une petite entreprise :

- suivre les incidents ;
- organiser les demandes ;
- classer les tickets ;
- relier les tickets au parc informatique ;
- préparer une base de connaissances.

## Limite

À cette étape, les catégories sont seulement préparées dans la documentation.

Elles seront réellement créées dans GLPI lorsque l’environnement sera installé et accessible.