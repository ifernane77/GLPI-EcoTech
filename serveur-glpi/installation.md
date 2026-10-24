# Installation de GLPI sur Debian 11

> État documentaire au 24 octobre 2026 : procédure de laboratoire et captures historiques conservées. Le projet EcoTech est une simulation. Ces traces ne certifient ni la disponibilité actuelle du service, ni un déploiement en production. Les commandes décrivent le travail documenté ; elles ne constituent pas un script de réinstallation validé.
> La procédure mentionne GLPI 10.0.25 ; la version installée reste à confirmer dans l’interface. La provenance et les commandes d’ajout du dépôt PHP 8.1 ne sont pas conservées. La modification des mots de passe par défaut n’est pas démontrée ; le tableau de bord initial affiche une alerte. Le mot de passe SQL publié auparavant a été neutralisé dans cette version, mais reste dans l’historique Git : s’il a été utilisé, le changer dans MariaDB et dans la configuration GLPI.

## 1. Présentation du projet

Ce mini-projet consiste à installer **GLPI** sur une machine virtuelle Debian 11.

L’objectif est de mettre en place un service informatique accessible depuis un navigateur, en utilisant une architecture classique :

* **Debian 11** : système d’exploitation serveur ;
* **Apache** : serveur web ;
* **PHP 8.1** : langage utilisé pour exécuter GLPI ;
* **MariaDB** : système de gestion de base de données ;
* **GLPI** : application web de gestion de parc informatique et de tickets.

---

## 2. Architecture utilisée

L’architecture fonctionne de la manière suivante :

```text
Utilisateur → Navigateur → Apache → PHP → GLPI → MariaDB
```

Explication :

* L’utilisateur accède à GLPI depuis un navigateur.
* Apache reçoit la requête web.
* PHP exécute le code de GLPI.
* GLPI lit et écrit ses données dans MariaDB.

---

## 3. Environnement technique

Machine utilisée :

* Type : machine virtuelle
* Système : Debian 11
* Serveur web : Apache
* Version PHP utilisée : PHP 8.1
* Base de données : MariaDB
* Application installée : GLPI

Preuve :

```text
Capture : ../preuves/installation-serveur/01_vm_debian.png
```

---

## 4. Installation du serveur web Apache

Commande utilisée :

```bash
apt install -y apache2
```

Explication :

Cette commande installe **Apache**, qui permet d’héberger des pages web et de rendre GLPI accessible depuis un navigateur.

Vérification :

```bash
systemctl status apache2
```

Preuve :

```text
Capture : ../preuves/installation-serveur/02_apache_php.png
```

---

## 5. Installation de PHP 8.1

PHP 8.1 a été installé afin d’exécuter l’application GLPI.

Commandes utilisées :

```bash
apt install -y php8.1 libapache2-mod-php8.1 php8.1-mysql
```

Explication :

* `php8.1` installe PHP ;
* `libapache2-mod-php8.1` permet à Apache d’utiliser PHP 8.1 ;
* `php8.1-mysql` permet à PHP de communiquer avec MariaDB.

Vérification :

```bash
php8.1 -v
ls /etc/apache2/mods-enabled/php*.load
```

Preuve :

```text
Capture : ../preuves/installation-serveur/03_php81_apache.png
```

---

## 6. Activation de PHP 8.1 dans Apache

Commandes utilisées :

```bash
a2dismod php7.4
a2enmod php8.1
systemctl restart apache2
```

Explication :

Apache utilisait encore PHP 7.4. J’ai donc désactivé le module PHP 7.4 et activé le module PHP 8.1 afin que GLPI fonctionne avec la bonne version de PHP.

Vérification :

```bash
ls /etc/apache2/mods-enabled/php*.load
```

Résultat attendu :

```text
/etc/apache2/mods-enabled/php8.1.load
```

---

## 7. Installation de MariaDB

Commande utilisée :

```bash
apt install -y mariadb-server
```

Explication :

MariaDB est le serveur de base de données. GLPI l’utilise pour stocker ses informations : utilisateurs, tickets, matériels, configurations, etc.

Vérification :

```bash
systemctl status mariadb
```

Preuve :

```text
Capture : ../preuves/installation-serveur/04_mariadb.png
```

---

## 8. Installation des extensions PHP nécessaires

Commande utilisée :

```bash
apt install -y php8.1-curl php8.1-gd php8.1-intl php8.1-mbstring php8.1-xml php8.1-zip php8.1-bz2 php8.1-ldap php8.1-apcu php8.1-opcache php8.1-bcmath
```

Explication :

Ces extensions ajoutent des fonctionnalités nécessaires à GLPI, par exemple la gestion des fichiers compressés, des images, du XML, des langues, ou encore la communication avec certains services.

Vérification :

```bash
php -m | grep -E "curl|gd|intl|mbstring|mysqli|xml|zip|ldap|apcu|bcmath"
```

Preuve :

```text
Capture : ../preuves/installation-serveur/05_extensions_php.png
```

---

## 9. Téléchargement et extraction de GLPI

Commandes utilisées :

```bash
cd /tmp
wget https://github.com/glpi-project/glpi/releases/download/10.0.25/glpi-10.0.25.tgz
tar -xvzf glpi-10.0.25.tgz
mv glpi /var/www/html/
```

Explication :

* Le fichier GLPI est téléchargé dans `/tmp`.
* L’archive est extraite.
* Le dossier `glpi` est déplacé dans `/var/www/html`, qui est le dossier utilisé par Apache pour afficher les sites web.

---

## 10. Attribution des droits au dossier GLPI

Commandes utilisées :

```bash
chown -R www-data:www-data /var/www/html/glpi
chmod -R 755 /var/www/html/glpi
```

Explication :

Apache fonctionne avec l’utilisateur `www-data`. Il faut donc donner les droits nécessaires à cet utilisateur pour que GLPI puisse fonctionner correctement.

Vérification :

```bash
ls -ld /var/www/html/glpi
```

Preuve :

```text
Capture : ../preuves/installation-serveur/06_dossier_glpi.png
```

---

## 11. Création de la base de données GLPI

Connexion à MariaDB :

```bash
mariadb -u root
```

Commandes SQL utilisées :

```sql
CREATE DATABASE glpi CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
CREATE USER 'glpiuser'@'localhost' IDENTIFIED BY '<MOT_DE_PASSE_SQL_A_DEFINIR>';
GRANT ALL PRIVILEGES ON glpi.* TO 'glpiuser'@'localhost';
FLUSH PRIVILEGES;
EXIT;
```

Explication :

* Une base de données nommée `glpi` est créée.
* Un utilisateur `glpiuser` est créé.
* Les droits sur la base `glpi` sont donnés à cet utilisateur.

Vérification :

```bash
mariadb -u root -e "SHOW DATABASES;"
```

Preuve :

```text
Capture : ../preuves/installation-serveur/07_base_glpi.png
```

---

## 12. Installation de GLPI depuis le navigateur

Adresse utilisée :

```text
http://localhost/glpi
```

Informations de connexion à la base :

```text
Serveur SQL : localhost
Utilisateur SQL : glpiuser
Mot de passe : <MOT_DE_PASSE_SQL_A_DEFINIR>
Base de données : glpi
```

Explication :

L’installation graphique permet de connecter GLPI à la base de données MariaDB et de finaliser la configuration de l’application.

Preuve :

```text
Capture de cette étape non conservée dans le dépôt. La connexion et le tableau de bord sont conservés aux étapes suivantes.
```

---

## 13. Connexion à GLPI

Identifiants par défaut :

```text
Utilisateur : glpi
Mot de passe : glpi
```

Après la première connexion, il est recommandé de modifier les mots de passe par défaut pour sécuriser l’application.

Preuves :

```text
Capture : ../preuves/installation-serveur/09_connexion_glpi.png
Capture : ../preuves/installation-serveur/10_tableau_de_bord_glpi.png
```

---

## 14. Suppression du dossier d’installation

Commande utilisée :

```bash
rm -rf /var/www/html/glpi/install
```

Explication :

Après l’installation, il faut supprimer le dossier d’installation afin d’éviter qu’une personne puisse relancer l’installation de GLPI.

Vérification :

```bash
ls /var/www/html/glpi
```

Preuve :

```text
Capture : ../preuves/installation-serveur/11_suppresion_install.png
```

---

## 15. Difficultés rencontrées

Pendant l’installation, plusieurs difficultés ont été rencontrées :

### Problème 1 : PHP 8.1 introuvable

Debian 11 propose PHP 7.4 par défaut. Il a donc fallu ajouter un dépôt externe afin d’installer PHP 8.1.

### Problème 2 : mauvais PATH root

La commande `dpkg` indiquait que certains programmes système étaient introuvables. Le problème venait du fait que le chemin système root ne contenait pas certains dossiers comme `/usr/sbin` et `/sbin`.

Correction utilisée :

```bash
export PATH=$PATH:/usr/local/sbin:/usr/sbin:/sbin
```

### Problème 3 : Apache utilisait encore PHP 7.4

Même après l’installation de PHP 8.1, Apache utilisait encore PHP 7.4.

Correction utilisée :

```bash
a2dismod php7.4
a2enmod php8.1
systemctl restart apache2
```

### Problème 4 : erreur sur la commande chown

Une erreur est apparue à cause d’une faute de frappe :

```text
www-date
```

au lieu de :

```text
www-data
```

Commande correcte :

```bash
chown -R www-data:www-data /var/www/html/glpi
```

---

## 16. Conclusion

Ce projet m’a permis de comprendre la mise en place d’une application web sur un serveur Linux.

J’ai appris à :

* installer et configurer Apache ;
* installer PHP et ses extensions ;
* installer MariaDB ;
* créer une base de données ;
* déployer une application web dans `/var/www/html` ;
* gérer les droits avec `chown` ;
* finaliser une installation depuis un navigateur ;
* produire une documentation technique avec des preuves.

Ce mini-projet correspond à une situation professionnelle de mise à disposition d’un service informatique.
