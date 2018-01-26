# GoBittrexDockerConfig
Docker config for setting up db, etc....

### Setup:

```bash
Download or clone config from Github
Install and Run Docker
run:
// Run container with docker-compose:
$ docker-compose -f docker-compose.yml up -d
// or with docker command:
$ docker run -p 3306:3306 --name <container_name> -e MYSQL_ROOT_PASSWORD=xxxx -d mysql
// Login to database using:
$ docker exec -it <container_name> mysql -h localhost -P 3306 -u root -p
// Use xxxx/xxxx as user/password credentials
```

```bash
Remove containers
run:
// Stop container if needed:
$ docker stop <container_name>
// Delete container if needed:
$ docker rm <container_name>
```
