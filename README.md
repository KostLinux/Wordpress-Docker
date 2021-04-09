# Wordpress Docker Compose For Local Web Site Development

Setup wordpress development environment via docker-compose.

By default it will save database mysql files to ./wp-db and wordpress files to ./wp-app

Official repository: https://github.com/nezhar/wordpress-docker-compose/

## Configuration

1. Clone this repository and change directory to repository

	```
	https://gitlab.com/itwebsolutions/docker-wordpress
	```

2. Change wordpress database and mariadb database variables in .env

	**Note:** Use this link to create secure passwords: https://passwordsgenerator.net/

	```
	IP=127.0.0.1
	DB_ROOT_PASSWORD=wordpress_user_password
	DB_NAME=wordpress

	```

## Setup

1. Build wordpress

- If you want to build without logs:

	`docker-compose up -d`

- If you want to see logs:

	`docker-compose up`

2. Go to http://127.0.0.1 and you will get in wordpress installation page

3. Setup your website name, username and password. Email can be random, for example: somemail@mail.com

4. Enjoy your development!

## Notes

Changes did from repository:

- Removed WP-CLI
- Removed PHPMyAdmin
- Change wordpress port listening from ${IP}:80:80 to 80:80
- Change db port listening from ${IP}:3306:3306 to 3306:3306

## Author
* **Christofher** - *Initial work* - [KostLinux](https://github.com/KostLinux)
