# Environnement technique documenté

| Élément | État documenté | Limite |
|---|---|---|
| Virtualisation | VirtualBox, deux VM décrites dans la procédure agent | Export des VM non présent dans le dépôt |
| Serveur | Debian 11, Apache, PHP 8.1, MariaDB, GLPI | Versions exactes à relever ; GLPI 10.0.25 est la version citée par la procédure |
| Client | Debian 11, GLPI Agent ; installateur 1.16 cité | Version installée et dernier inventaire à relever |
| Réseau | Accès par pont ; serveur 192.168.1.34 lors de l’essai | Adresse actuelle à vérifier |
| Client inventorié | Debian-Client-GLPI-Agent | Visible dans l’entité racine, rattachement EcoTech non démontré |
| Accès web | localhost/glpi sur le serveur ; IP du serveur depuis le client | Aucune disponibilité actuelle garantie par les captures |

## Vérification avant démonstration

Démarrer les VM, relever leur identité et leurs adresses, vérifier les services puis l’accès web et effectuer un inventaire. Conserver les sorties utiles sans secrets.

```bash
hostnamectl
ip -br address
systemctl status apache2 mariadb --no-pager
php -v
```

Sur le client, relever la version de l’agent et vérifier l’URL configurée avant de déclencher un inventaire. Voir les [procédures techniques](installation-glpi.md) et la [procédure d’accès](procedure-acces-vm.md).
