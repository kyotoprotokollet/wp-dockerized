# WP-Dockerized.
- A Wordpress starting point based on Docker and [Bedrock](https://roots.io/bedrock/).
- PHP 7, MariaDB, Nginx
- [WP-CLI](http://wp-cli.org/) support
- phpMyAdmin
- [Mailcatcher](https://mailcatcher.me/)

## Requirements:
* Docker
* Composer
---------------
### Installation instructions
* Clone this repository
* Copy .env.example to .env and set preferred database name and database prefix:
	* DB_NAME - Desired database name
    * DB_PREFIX - Desired database prefix
    * Root user and password is setup so you can leave these or create a new user/pass and set those here
	* Generate salts and keys for Wordpress [here](https://api.wordpress.org/secret-key/1.1/salt/) and fill those in
* From root folder:
    - `composer install`
    - `docker-compose up`

+ Visit [http://localhost](http://localhost) for Wordpress
+ Visit [http:/localhost:70](http:/localhost:70) for PHPMyAdmin (default user & pass is root/root)
+ Visit [http:/localhost:1080](http:/localhost:1080) for Mailcatcher

## Guide
* This setup is based on the [Bedrock boilerplate](https://roots.io/bedrock/).
* Use composer to manage dependencies (Wordpress, themes, plugins)
