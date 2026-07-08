# Procédure de traitement d’un ticket — GLPI EcoTech

## Objectif

Ce document prépare la procédure de traitement d’un ticket dans GLPI EcoTech.

À cette étape, la procédure est rédigée en documentation.

Elle sera appliquée plus tard dans GLPI lorsque l’outil sera installé et configuré.

---

## Contexte

EcoTech est une petite entreprise qui utilise plusieurs équipements informatiques :

- PC fixes ;
- PC portables ;
- téléphones professionnels ;
- imprimante / scanner ;
- Livebox ;
- Google Drive ;
- mails professionnels.

Les incidents et demandes peuvent concerner le matériel, les accès, les documents ou le réseau.

---

## Étape 1 — Déclarer le ticket

Un utilisateur signale un problème ou une demande.

Exemples :

- imprimante qui ne fonctionne plus ;
- PC lent ;
- accès Google Drive impossible ;
- document introuvable ;
- téléphone professionnel abîmé ;
- problème de connexion Internet.

Informations à renseigner :

- nom du demandeur ;
- date de la demande ;
- type de demande ;
- description du problème ;
- équipement concerné si besoin ;
- urgence ressentie.

---

## Étape 2 — Qualifier le ticket

Le ticket doit être classé pour mieux le traiter.

Éléments à définir :

- type : incident ou demande ;
- catégorie ;
- priorité ;
- utilisateur concerné ;
- équipement concerné.

Exemples de catégories :

- matériel ;
- impression ;
- réseau ;
- cloud / Google Drive ;
- documents ;
- sauvegarde ;
- application EcoTech.

---

## Étape 3 — Affecter le ticket

Le ticket doit être affecté à une personne ou un groupe.

Dans le projet GLPI EcoTech, l’affectation prévue est simple :

- tickets utilisateurs vers le support informatique ;
- tickets matériels vers le technicien ;
- tickets documents ou accès vers le support ou l’administrateur ;
- tickets importants visibles par les gérants si besoin.

---

## Étape 4 — Traiter le ticket

Le technicien analyse le problème.

Il peut :

- demander des précisions ;
- vérifier l’équipement ;
- proposer une solution ;
- indiquer une action réalisée ;
- changer le statut du ticket.

Exemple :

Un employé signale que l’imprimante ne répond plus.

Le support vérifie la connexion, le câble, le réseau et le statut de l’imprimante.

---

## Étape 5 — Documenter la solution

La solution doit être notée dans le ticket.

Cela permet de garder une trace.

Exemples de solutions :

- redémarrage de l’imprimante ;
- reconnexion au Wi-Fi ;
- partage Google Drive corrigé ;
- document déplacé dans le bon dossier ;
- remplacement d’un câble ;
- réinitialisation d’un accès.

---

## Étape 6 — Clôturer le ticket

Le ticket peut être clôturé lorsque le problème est résolu.

Avant la clôture, il faut vérifier :

- que la demande a bien été traitée ;
- que l’utilisateur peut de nouveau travailler ;
- que la solution est notée ;
- que le statut est correct.

---

## Statuts prévus

Les statuts simples prévus sont :

| Statut | Signification |
|---|---|
| Nouveau | Ticket déclaré |
| En cours | Ticket pris en charge |
| En attente | Besoin d’une information ou d’une action externe |
| Résolu | Solution appliquée |
| Clos | Ticket terminé |

---

## Remarque personnelle

Cette procédure me permet de préparer l’utilisation de GLPI avant de créer les tickets réellement dans l’outil.

Elle me servira aussi à expliquer la démarche de support informatique pour l’épreuve E5.