# Installation GLPI — point d’entrée

GLPI a été installé et son interface est visible dans les captures conservées. L’ancienne préparation à l’installation est remplacée par les traces techniques disponibles.

- [Installation du serveur Debian / Apache / PHP / MariaDB / GLPI](serveur-glpi/installation.md).
- [Installation et configuration du client GLPI Agent](agent-glpi/installation.md).
- [Environnement et vérifications avant démonstration](environnement-debian.md).
- [Captures serveur](preuves/installation-serveur/README.md).
- [Captures agent](preuves/inventaire-agent/README.md).

## Limites de reproductibilité

La commande d’ajout du dépôt PHP 8.1 n’est pas documentée. La capture de l’assistant d’installation navigateur n’est pas conservée. Les versions réellement installées doivent être relevées dans le laboratoire. Les procédures décrivent un travail historique ; aucune nouvelle réinstallation n’a été testée lors de la révision documentaire.

## Accès et secrets

La procédure SQL utilise désormais un emplacement fictif pour le mot de passe. Un ancien mot de passe reste présent dans l’historique Git : le changer s’il a été utilisé. Le changement des comptes GLPI par défaut n’est pas démontré par les preuves présentes.
