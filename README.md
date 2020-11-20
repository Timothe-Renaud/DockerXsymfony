# { nginx X php7.4 X mysql8 X node } -> docker-network
Fast lightweight Docker network using PHP MySQL Nginx and Node

Docker said I'm fast as fuck boyyyyyyyyyy!

- clone de project from: https://codeload.github.com/GaryClarke/nginx-php7.4-mysql8-node-docker-network/zip/master

```
git clone https://codeload.github.com/GaryClarke/nginx-php7.4-mysql8-node-docker-network/zip/master

code .
```

- run this commande 

```
docker-compose up -d --build  
```

- visite: http://localhost:8080/
- Pour installé Symfony
- Supp le repertoir app/public car le skeleton de symfony vas etre installé dans le rep "App"
-  ouvrire le container php74 en bash pour commncé l'installation de Symfony

```
docker exec -it php74-container bash
  
```
-- php74 etant le nom du neud de container forment le stack logik

- Install le skelette -> symfony/skeleton  via :

```
composer create-project symfony/skeleton .
```
- Re-visite: http://localhost:8080/