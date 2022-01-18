# Series !
Projet présenté dans les cours vidéos sur Symfony5 à l'ENI.

## Instructions d'installation
Dans le terminal : 
```bash
# on se déplace dans notre répertoire web
cd /Wamp64/www/
# clone ce projet depuis github
git clone https://github.com/gsylvestre/serie-symfony-eni
# on se déplace dans le nouveau répertoire créé  
cd serie-symfony-eni/
# télécharge les dépendances composer
composer install  
# crée la bdd telle que configurée dans le fichier .env
php bin/console doctrine:database:create
# crée les tables
php bin/console doctrine:schema:update --force
# importe les données de séries et de saisons
php bin/console doctrine:fixtures:load
```

Puis naviguer vers http://localhost/serie-symfony-eni/public/# serie
