# Parc informatique enregistré — EcoTech

## Neuf fiches de simulation visibles

| Nom dans GLPI | Type visible | Précision |
|---|---|---|
| ECO-PC-ADM-01 | PC fixe | Dell OptiPlex, bureau administratif |
| ECO-PC-GER-01 | PC portable | HP ProBook, bureau des gérants |
| ECO-MAC-GER-02 | PC portable | Apple MacBook Air, bureau des gérants |
| ECO-PC-SUP-01 | PC portable | Lenovo ThinkPad, bureau support |
| ECO-IMP-ADM-01 | Imprimante | Associée au ticket 4 |
| ECO-NET-LIVEBOX-01 | Matériel réseau | Associé au ticket 8 |
| ECO-TEL-GER-01 | Téléphone | Fiche visible dans la liste globale |
| ECO-TEL-GER-02 | Téléphone | Fiche visible dans la liste globale |
| ECO-TEL-TER-01 | Téléphone | Associé au ticket 10 |

Les neuf fiches sont affichées « En service » dans EcoTech. Les ordinateurs portent des numéros de série préfixés `SIM-` : ces données représentent le scénario, pas un recensement certifié du matériel physique de l’entreprise.

## Fiche détaillée conservée

`ECO-PC-ADM-01` : utilisateur Administratif EcoTech, groupe Employés, responsable technique Support EcoTech, groupe technique Support informatique, numéro d’inventaire `INV-ECO-PC-ADM-01`, localisation bureau administratif et un ticket associé. Le système d’exploitation des quatre postes n’est pas renseigné dans la capture de liste ; ne pas annoncer une répartition Windows/macOS non vérifiée.

## Client Debian inventorié automatiquement

`Debian-Client-GLPI-Agent` apparaît comme machine VirtualBox sous Debian GNU/Linux 11 dans une capture distincte, avec processeur et identifiant remontés. Les captures suivantes montrent les logiciels et composants. Ce client est visible dans l’entité racine ; son rattachement aux fiches EcoTech n’est pas démontré. Il n’est pas compté parmi les neuf fiches simulées.

## Compléments utiles

Conserver un export du parc et les fiches imprimante, Livebox et téléphone terrain avec leurs relations aux tickets. Conserver la source et la date du dernier inventaire du client Debian. Le serveur est documenté comme VM d’hébergement ; aucune fiche `SRV-GLPI-TEST` n’est démontrée dans le parc EcoTech.

[Preuves parc](preuves/parc/README.md) et [preuves agent](preuves/inventaire-agent/README.md).
