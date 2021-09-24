<!-- GETTING STARTED -->
## Getting Started

You can use Docker Compose to easily run WordPress in an isolated environment built with Docker containers. This quick-start guide demonstrates how to use Compose to set up and run WordPress. Before starting, make sure you have Compose installed.

### Instalation
1. Create directory where you want to clone repository
```sh
mkdir yourproject && cd yourproject
```
2. Clone the repo on directory
```sh
git clone https://github.com/kutia-software-company/wordpress-with-docker.git .
```
3. Copy from environment example to environment
```sh 
cp .env.example .env
```

4. Run docker compose
```sh
docker-compose up -d --build
```

open in browser:
```
http://locahost:8000
```

Inside src folder you can see wordpress contents here you can work your plugin or theme

![Select Language](https://docs.docker.com/samples/images/wordpress-lang.png)

![Setup](https://docs.docker.com/samples/images/wordpress-welcome.png)

if you want to access in phpmyadmin:
```
http://localhost:8181/
```
username: wordpress <br>
password: wordpress

you can change all information in .env file

### Shutdown and cleanup
The command `docker-compose down` removes the containers and default network, but preserves your WordPress database.

The command `docker-compose down --volumes` removes the containers, default network, and the WordPress database.