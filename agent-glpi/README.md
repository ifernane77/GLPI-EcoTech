# Projet GLPI Agent — BTS SIO SLAM

> État documentaire au 24 octobre 2026 : procédure de laboratoire et captures historiques conservées. Le projet EcoTech est une simulation. Ces traces ne certifient ni la disponibilité actuelle du service, ni un déploiement en production. Les commandes décrivent le travail documenté ; elles ne constituent pas un script de réinstallation validé.

## Présentation

Ce projet consiste à mettre en place un inventaire automatique entre un poste client Debian et un serveur GLPI à l’aide de **GLPI Agent**.

L’objectif est de faire remonter automatiquement un poste client dans GLPI avec ses informations matérielles, logicielles et système.

---

## Architecture du projet

```text
VM 1 : Serveur GLPI
Debian 11 + Apache + PHP + MariaDB + GLPI

        ↑ Remontée d’inventaire

VM 2 : Poste client
Debian 11 + GLPI Agent
```

---

## Objectif

Mettre en place une communication entre un poste client Debian et un serveur GLPI afin que le poste soit automatiquement inventorié dans GLPI.

---

## Travail réalisé

* Utilisation d’une VM Debian avec GLPI installé.
* Création d’une deuxième VM Debian comme poste client.
* Configuration réseau des deux VM en accès par pont.
* Vérification de la communication entre le client et le serveur avec `ping`.
* Activation de l’inventaire dans GLPI.
* Installation de GLPI Agent sur le poste client Debian.
* Configuration de l’adresse du serveur GLPI dans l’agent.
* Accès à l’interface locale de GLPI Agent.
* Forçage d’un inventaire.
* Vérification de la remontée du poste dans GLPI.
* Consultation des logiciels et composants détectés.

---

## Compétences travaillées

Ce projet m’a permis de travailler plusieurs compétences utiles en BTS SIO :

* mise en place d’un service informatique ;
* configuration réseau entre deux machines virtuelles ;
* installation et configuration d’un agent d’inventaire ;
* gestion d’un parc informatique avec GLPI ;
* vérification de la communication client-serveur ;
* documentation technique ;
* production de preuves professionnelles.

---

## Captures d’écran

Les preuves du projet sont disponibles dans le dossier :

```text
../preuves/inventaire-agent/
```

Liste des captures :

```text
01-reseau-vm-serveur-glpi.png
02-creation&reseau-vm-client.png
03-ip-serveur-glpi.png
04-ping-client-vers-serveur.png
05-activation-inventaire-glpi.png
06-installation-glpi-agent.png
07-interface-locale-agent.png
08-force-inventory.png
09-poste-detecte-dans-glpi.png
10-logiciels-detectes.png
11-composants-detectes.png
```

---

## Documentation technique

La procédure complète est disponible dans le fichier :

```text
installation.md
```

---

## Conclusion

Ce mini-projet montre la mise en place d’un inventaire automatique avec GLPI Agent. Il permet de comprendre le fonctionnement d’un outil de gestion de parc informatique dans une logique client-serveur.
