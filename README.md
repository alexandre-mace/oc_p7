# Snowtricks

Web Service with API REST, 7th project from OpenClassroom's class

## Requirements 
* MySQL : https://www.mysql.com/fr/

* PHP : http://php.net/manual/fr/intro-whatis.php

* Apache : https://www.apache.org/

## Installation 
* Clone the repository and open it.

```
  git clone https://github.com/alexandre-mace/oc_p7.git
  cd oc_p7
```

* Install dependencies.

  `install update`

## Configuration
* Customize the .env file

#### doctrine
  `DATABASE_URL="mysql://db_user:db_password@127.0.0.1:3306/db_name"`

* Create database 

  `php bin/console doctrine:database:create`

* Get tables 

```
  php bin/console doctrine:make:migration
  php bin/console doctrine:migrations:migrate
```

* Get data

  `php bin/console doctrine:fixtures:load`

## Tests
```
* run in console `./bin/phpunit` and results will show up in console
```