[![Build Status](https://travis-ci.com/Nyhn/Projet9.svg?branch=master)](https://travis-ci.com/Nyhn/Projet9)  [![Coverage Status](https://coveralls.io/repos/github/Nyhn/Projet9/badge.svg)](https://coveralls.io/github/Nyhn/Projet9)

# MyERP

## Organisation du répertoire

*   `doc` : documentation
*   `docker` : répertoire relatifs aux conteneurs _docker_ utiles pour le projet
    *   `dev` : environnement de développement
*   `src` : code source de l'application


## Environnement de développement

Les composants nécessaires lors du développement sont disponibles via des conteneurs _docker_.
L'environnement de développement est assemblé grâce à _docker-compose_
(cf docker/dev/docker-compose.yml).

Il comporte :

*   une base de données _PostgreSQL_ contenant un jeu de données de démo (`postgresql://127.0.0.1:9032/db_myerp`)



### Lancement

    cd docker/dev
    docker-compose up


### Arrêt

    cd docker/dev
    docker-compose stop


### Remise à zero

    cd docker/dev
    docker-compose stop
    docker-compose rm -v
    docker-compose up
    
### Travails effectués ( Date : 14/10/2020 )

Voir pdf `TravailEffectue.pdf`