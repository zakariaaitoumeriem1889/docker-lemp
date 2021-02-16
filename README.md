# Kit Symfony 5 Docker

## Conteneur
- nginx
- php-fpm 8 (php 8)
- MariaDB
- PhpMyAdmin
- MailDev

# Installation
Pour démarrer docker et se connecter avec le conteneur:
`docker-compose up --build`<br/><br/>
Pour Créer le projet symfony:<br/>
- Créer le répertoire app: `mkdir app`
- `docker-compose exec php bash`
- `composer create-project symfony/skeleton .` <br/> (Pour les projets Microservices)
- `composer create-project symfony/web-skeleton .` <br/> (Pour les applications web traditionnels)
- `chmod -R 777 .`
- Pour la base de données:<br/>
  `DATABASE_URL=mysql://root:root@mysql:3306/SymfonyDB?serverVersion=5.7`

# Prêt!
- `http://localhost`
- `http://localhost:8081/` (phpmyadmin)
- `http://localhost:1500/` (maildev)
