# serie
<p align="center">
  <img width="700" height="350" src="https://github.com/christanvt/serie/blob/989280b4360b5eca8c4b0c26c67dbde77eae83e7/public/img/screenshotSerie.png">
</p>


<p align="center">
  <a href="https://symfony.com/"><img height="30" src="https://img.shields.io/badge/Symfony-lightgrey?style=flat&logo=symfony&logoColor=white&labelColor=black&link=http://left&link=http://right"></a>
  <a href="https://mariadb.org/"><img height="30" src="https://img.shields.io/badge/MySQL-lightgrey?style=flat&logo=MySQL&logoColor=white&labelColor=red"></a>
  <a href="https://www.php.net/"><img height="30" src="https://img.shields.io/badge/Php-lightgrey?style=flat&logo=php&logoColor=white&labelColor=8892BF"></a>
  <a href="https://getcomposer.org/"><img height="30" src="https://img.shields.io/badge/Composer-lightgrey?style=flat&logo=composer&logoColor=44f&labelColor=eee&Color=red"></a>
</p>


## Install

### Clone and install required packages :

    git clone https://github.com/christanvt/serie.git
    cd serie
    composer install

### Configure database access (change db_user and db_password to your needs) :

    echo "APP_ENV=dev" > .env.local
    echo "# APP_DEBUG=0" > .env.local
    echo "APP_SECRET=secret" >> .env.local
    echo "DATABASE_URL=mysql://db_user:db_password@127.0.0.1:3306/serie" >> .env.local

### Create database :

    php bin/console doctrine:database:create
    php bin/console doctrine:migrations:migrate

### Load required fixtures :

    php bin/console doctrine:fixtures:load required

## Test fixtures

### Load test fixtures :

    php bin/console doctrine:fixtures:load

## Test the site


<a href="https://series.devformatic.fr/">series.devformatic.fr</a>
