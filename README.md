# Stockage--products-
# Projet de Réparation de Cartes Électroniques

Ce projet est une application Java Swing qui permet de gérer les réparations de cartes électroniques. L'application permet d'ajouter, modifier, supprimer et afficher les détails des cartes électroniques en réparation.

## Fonctionnalités

- **Ajouter une carte électronique** : Ajoutez les détails d'une nouvelle carte électronique à la base de données.
- **Modifier une carte électronique** : Modifiez les informations d'une carte électronique existante.
- **Supprimer une carte électronique** : Supprimez une carte électronique de la base de données.
- **Afficher une carte électronique** : Affichez les détails d'une carte électronique en recherchant par son numéro de série (S/N).

## Structure du Projet

- `POPPP.java` : Classe principale contenant l'interface utilisateur et les actions des boutons.
- `Connec.java` : Classe de connexion à la base de données MySQL.

## Prérequis

- Java Development Kit (JDK)
- MySQL
- IDE Java (comme Eclipse ou IntelliJ IDEA)

## Configuration de la Base de Données

1. Assurez-vous d'avoir MySQL installé et en cours d'exécution.
2. Créez une base de données nommée `reparation_carte_electroniquenique`.
3. Créez une table `cartes_electroniques` avec la structure suivante :

```sql
CREATE TABLE `cartes_electroniques` (
  `sn` VARCHAR(255) NOT NULL,
  `model` VARCHAR(255) NOT NULL,
  `num_defaut` VARCHAR(255) NOT NULL,
  `type_defaut` VARCHAR(255) NOT NULL,
  `composant_defaut` VARCHAR(255) NOT NULL,
  PRIMARY KEY (`sn`)
);

