# Un site de TO-DO List encryptant email et hashant mot de passe

Ceci est une façon de faire l'exercice avec Symfony 6.2.




## Pré-requis
- composer v2
- PHP >= 8.1
- Une base de données MySQL
## Fichiers importants à regarder

- src/Controller
- src/Entity
- src/Form
- src/Repository/UserRepository.php ==> fonction loadUserByIdentifier()
- templates
- config/packages/security.yaml


## Variables d'environnement

Vous aurez besoin de créer un fichier .env.local avec les données suivantes :

`DATABASE_URL`

`IV`

`KEY`


## Installation

1. Cloner le projet
2. Faire la comande `composer install`
3. Assurez-vous d'avoir créer le .env.local mentionné à l'étape précédente
4. Créer la base données : `php bin/console doctrine:database:create`
5. Effectuer les migrations : `php bin/console doctrine:migrations:migrate`
