# GLPI EcoTech — dossier de support informatique

GLPI EcoTech est une simulation professionnelle de support informatique fondée sur le contexte d’une petite entreprise du BTP à Saint-Pierre, La Réunion. Ce dépôt conserve la documentation, les captures d’un environnement GLPI utilisé et les limites des preuves disponibles pour E5.

## Réalisations documentées

| Domaine | État étayé par les documents et captures |
|---|---|
| Serveur | GLPI accessible sur une VM Debian 11 ; installation Apache, PHP et MariaDB documentée |
| Agent | Client Debian séparé, configuration réseau et remontée d’inventaire documentées |
| Organisation | Entité EcoTech, cinq comptes EcoTech, quatre groupes ; habilitation Technician du support |
| Patrimoine | Neuf fiches d’équipements simulés, dont une fiche administrative détaillée |
| Support | Huit tickets visibles : six clos, un résolu, un en cours ; détails conservés pour trois incidents |
| Connaissances | Procédure de déclaration lisible ; article Google Drive visible dans une liste |

Ces preuves décrivent des états historiques du laboratoire. Elles ne démontrent pas un service en production chez EcoTech, le traitement réel de tous les scénarios envisagés ou une disponibilité actuelle. Les équipements simulés et le client réellement inventorié par agent sont distingués.

## Parcours de lecture

1. [Présentation et périmètre](presentation-projet.md).
2. [Installation serveur](serveur-glpi/installation.md) et [inventaire par agent](agent-glpi/installation.md).
3. [Organisation](organisation-glpi.md), [utilisateurs et droits](utilisateurs-et-droits.md), [parc](inventaire-parc.md).
4. [Registre des tickets](gestion-des-tickets.md) et [procédure de support](gestion-du-support.md).
5. [Index des preuves par thème](preuves/README.md).
6. [Présentation pour le portfolio](portfolio/presentation-portfolio-glpi.md).
7. [Compte rendu et preuves à compléter](compte-rendu-coherence.md).

## Traçabilité

La révision documentaire du 24 octobre 2026 s’appuie sur l’état `661422d` du 16 août 2026 et sur les captures déjà présentes. Elle ne correspond à aucune nouvelle intervention dans GLPI. Voir le [journal de traçabilité](journal-de-bord.md).
