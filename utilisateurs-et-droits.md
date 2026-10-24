# Utilisateurs, groupes et habilitations

## Comptes constatés

| Identifiant | Nom ou usage visible | Profil démontré |
|---|---|---|
| admin.ecotech | Administratif | Habilitation à conserver ; ce nom ne prouve pas des droits administrateur |
| gerant1.ecotech | Gérant 1 | Non démontré par une capture d’habilitation |
| gerant2.ecotech | Gérant 2 | Non démontré par une capture d’habilitation |
| support.ecotech | Support | Technician, entité EcoTech |
| terrain.ecotech | Terrain | Habilitation à conserver |
| glpi | Compte d’administration GLPI | Session Super-Admin visible dans les captures d’administration |

La capture `04-habilitation-support.png` montre une habilitation enregistrée Technician dans EcoTech. Le choix Self-Service dans le formulaire d’ajout n’est pas une deuxième habilitation enregistrée.

## Groupes constatés

- EcoTech - Employés.
- EcoTech - Gérants.
- EcoTech - Prestataires.
- EcoTech - Support informatique.

La liste les rattache à l’entité racine. La composition complète et la récursivité restent à capturer. La fiche du PC administratif associe le groupe Employés et le groupe technique Support informatique ; cela ne prouve pas les appartenances des comptes.

## Vérifications à conserver

1. Ouvrir chaque compte et capturer ses habilitations : profil, entité et récursivité.
2. Ouvrir chaque groupe utilisé et capturer ses membres et son périmètre.
3. Tester avec un demandeur la création et le suivi de ses tickets, puis constater ses limites d’accès au parc et aux autres tickets.
4. Tester avec le support la prise en charge et la résolution d’un ticket dans EcoTech.
5. Consigner date, compte testé, résultat obtenu et capture ; ne pas publier de mot de passe.

Les anciens noms prévisionnels `gerant01`, `administratif01` ou `support01` ne sont pas les identifiants montrés par les captures. Les termes demandeur et gérant décrivent ici des usages, sans présumer des noms exacts des profils configurés.

[Preuves conservées](preuves/utilisateurs-profils/README.md).
