# Sécurisation — éléments démontrés et contrôles à effectuer

## Éléments disponibles

- Compte support avec une habilitation Technician dans EcoTech.
- Procédure serveur décrivant la suppression du dossier d’installation ; capture conservée sous son nom historique `11_suppresion_install.png`.
- Fiches du parc et tickets pour tracer les incidents de la simulation.

Ces éléments ne démontrent pas une politique de sécurité déployée dans l’entreprise.

## Contrôles restant à étayer

| Contrôle | État de preuve | Comment le documenter |
|---|---|---|
| Comptes GLPI par défaut | Le tableau de bord initial affiche une alerte | Vérifier les comptes, changer les mots de passe conservés et capturer l’état sans exposer les secrets |
| Secret SQL ancien | Valeur neutralisée dans la documentation actuelle, encore présente dans l’historique | Si utilisée, changer le secret dans MariaDB et la configuration GLPI ; tester l’accès |
| Moindre privilège | Habilitation support visible ; autres profils non démontrés | Capturer les habilitations et tester les limites d’un demandeur |
| Accès HTTP | HTTP visible dans le laboratoire | Décrire le périmètre de test ; ne pas revendiquer HTTPS |
| Sauvegarde et restauration | Non démontrées | Conserver procédure, résultat de sauvegarde et test de restauration isolé |
| Mises à jour et antivirus des postes | Non démontrés | Relevés et résultats réels seulement si ces actions sont effectuées |

Ne conserver aucun mot de passe dans les captures ou exports publics. Les versions historiques Debian/PHP sont décrites comme environnement du projet ; aucune actualisation de l’environnement n’a été effectuée lors de la révision documentaire.
