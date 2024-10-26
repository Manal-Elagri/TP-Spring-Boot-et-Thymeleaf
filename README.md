# TP : Développement d'une application CRUD avec Spring Boot et Thymeleaf

Ce projet est une application Web CRUD simple utilisant Spring Boot et Thymeleaf. Il permet de gérer des entités utilisateur en utilisant une base de données MySQL.

## Prérequis

- Java 8 ou version ultérieure
- Maven
- MySQL

## Installation

1. **Configurer la base de données** : 
   - Créez une base de données MySQL nommée \`thymeleaf\`.
   - Mettez à jour les informations de connexion dans le fichier \`application.properties\` :
     \`\`\`properties
     spring.datasource.url = jdbc:mysql://localhost:3306/thymeleaf
     spring.datasource.username = <votre_nom_d_utilisateur>
     spring.datasource.password = <votre_mot_de_passe>
     \`\`\`

## Lancer l'application

1.Premier methode : Dans le terminal, exécutez la commande suivante pour démarrer l'application :
\`\`\`bash
mvn spring-boot:run
\`\`\`

2.Deuxieme methode : Dans IntelliJ IDEA, Ouvrire le code et lancer la classe main "Application"

3.Accédez à l'application dans votre navigateur à l'URL [http://localhost:8080](http://localhost:8080).

## Fonctionnalités

- **Création** d'un utilisateur
- **Lecture** des utilisateurs existants
- **Mise à jour** d'un utilisateur
- **Suppression** d'un utilisateur

## Structure du Projet

- **Dépendances Maven** : Les dépendances nécessaires, y compris \`spring-boot-starter-data-jpa\`, \`spring-boot-starter-thymeleaf\`, et \`mysql-connector-java\`, sont définies dans \`pom.xml\`.
- **Couche DAO** : Utilise Spring Data JPA pour les opérations CRUD via l'interface \`CrudRepository\`.
- **Contrôleur** : \`UserController\` gère les routes HTTP pour les opérations CRUD.
- **Vues Thymeleaf** : Les modèles HTML sont situés dans \`src/main/resources/templates\`.

### Ajouter un utilisateur
Accédez à [http://localhost:8080/signup](http://localhost:8080/signup) pour ajouter un nouvel utilisateur.

### Mettre à jour un utilisateur
Cliquez sur \"Edit\" dans la liste des utilisateurs pour modifier les informations d'un utilisateur existant.

### Supprimer un utilisateur
Cliquez sur \"Delete\" pour supprimer un utilisateur de la base de données.

## Auteur

Réalisé dans le cadre d'un TP sous la supervision du Mr. Mohamed Lachgar.

