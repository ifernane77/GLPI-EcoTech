# Accéder au laboratoire GLPI

## Informations connues

- Virtualisation documentée : VirtualBox.
- Deux VM : serveur GLPI sous Debian 11 et client `Debian-Client-GLPI-Agent`.
- Adresse serveur au moment des essais agent : `192.168.1.34`.
- GLPI : `http://localhost/glpi` depuis le serveur, ou `http://<IP_SERVEUR>/glpi` depuis une machine autorisée du réseau.
- Interface locale agent : `http://localhost:62354` depuis le client.

Le nom exact de la VM serveur et le compte Linux utilisé ne sont pas confirmés par cette documentation. Les vérifier dans le laboratoire ; aucun mot de passe ne doit être ajouté au dépôt.

## Procédure de vérification

1. Ouvrir VirtualBox et identifier les deux VM.
2. Vérifier leur configuration réseau, puis les démarrer.
3. Se connecter avec les comptes conservés hors du dépôt.
4. Relever le nom et l’adresse du serveur avec `hostnamectl` et `ip -br address`.
5. Vérifier Apache et MariaDB, puis ouvrir GLPI dans le navigateur.
6. Se connecter avec le compte adapté au test ; vérifier l’entité sélectionnée.
7. Sur le client, vérifier l’adresse cible de l’agent et la communication réseau avant l’envoi d’inventaire.

Conserver la date du test et une capture d’accès réussie. L’ancienne adresse n’est pas une réservation IP démontrée. Voir [environnement](environnement-debian.md).
