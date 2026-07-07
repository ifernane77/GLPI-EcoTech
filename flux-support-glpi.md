# Flux de support — GLPI EcoTech

## Objectif

Ce document décrit les flux de support prévus pour GLPI EcoTech.

L’objectif est d’expliquer comment une demande ou un incident peut être signalé, suivi et résolu avec GLPI.

---

## Principe général

Avant GLPI, les informations sont dispersées entre :

- WhatsApp ;
- emails ;
- échanges oraux ;
- Google Drive ;
- PC personnels.

Avec GLPI, les incidents et demandes pourront être centralisés sous forme de tickets.

---

## 1. Flux — Déclaration d’un incident

### Exemple

L’imprimante ne fonctionne plus.

### Étapes prévues

1. L’utilisateur constate le problème.
2. Il crée un ticket dans GLPI ou demande au support de le saisir.
3. Le ticket est classé dans la catégorie adaptée.
4. Le ticket est associé à l’équipement concerné.
5. Le technicien analyse le problème.
6. Une solution est proposée.
7. Le ticket est résolu.
8. Le ticket est clôturé.

### Résultat attendu

L’incident est tracé et peut être retrouvé plus tard.

---

## 2. Flux — Demande d’accès

### Exemple

Un employé demande l’accès à un dossier Google Drive.

### Étapes prévues

1. L’utilisateur formule une demande.
2. Le ticket est créé dans GLPI.
3. Le ticket est classé dans la catégorie `Cloud / Google Drive`.
4. Le responsable vérifie si l’accès est justifié.
5. L’accès est accordé ou refusé.
6. La réponse est ajoutée dans le ticket.
7. Le ticket est clôturé.

### Résultat attendu

La demande est suivie et documentée.

---

## 3. Flux — Incident matériel

### Exemple

Un téléphone professionnel est abîmé.

### Étapes prévues

1. L’utilisateur signale le problème.
2. Le ticket est créé dans GLPI.
3. Le ticket est associé au téléphone concerné.
4. Le matériel est vérifié.
5. Une décision est prise : réparation, remplacement ou mise hors service.
6. Le statut du ticket est mis à jour.
7. Le ticket est clôturé.

### Résultat attendu

Le problème matériel est lié à l’équipement dans GLPI.

---

## 4. Flux — Problème réseau

### Exemple

La connexion Internet est instable.

### Étapes prévues

1. L’utilisateur signale le problème.
2. Le ticket est créé dans GLPI.
3. Le ticket est classé dans la catégorie `Réseau`.
4. L’équipement `BOX-01` est associé au ticket.
5. Les premières vérifications sont réalisées.
6. Une solution est documentée.
7. Le ticket est clôturé.

### Résultat attendu

Le problème réseau est suivi et peut être analysé si le problème revient.

---

## 5. Flux — Demande documentaire

### Exemple

Un devis est introuvable.

### Étapes prévues

1. L’utilisateur crée une demande.
2. Le ticket est classé dans la catégorie `Documents`.
3. La recherche est effectuée dans les emplacements connus.
4. Une réponse est apportée à l’utilisateur.
5. Si nécessaire, une procédure de classement est ajoutée.
6. Le ticket est clôturé.

### Résultat attendu

La demande est tracée et permet d’améliorer l’organisation documentaire.

---

## Schéma simple du flux de ticket

```mermaid
flowchart TD
    A[Utilisateur EcoTech] --> B[Création du ticket GLPI]
    B --> C[Catégorie du ticket]
    C --> D[Association à un équipement ou service]
    D --> E[Analyse du problème]
    E --> F[Réponse ou intervention]
    F --> G[Résolution]
    G --> H[Clôture du ticket]
    H --> I[Historique conservé dans GLPI]