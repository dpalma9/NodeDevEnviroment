**USER MANUAL**
=================

Overview
-------
This is personal project to mount a simple dev arch with Node + MySQL.

Pre-requirements
---------
Docker and docker-compose.

Requirements
---------
Place your data on the node folder


How to
----------
Delete the Entrypoint line from the NodeJS Dockerfile and uncomment the command line on the docker-compose node service.

Then, just run it:

```bash
$ docker-compose up -d 
```

Help commands
---------

To stop the project:

```
$ docker-compose stop
```

To delete the project:

```bash
docker-compose stop
docker-compose rm
``` 

To rebuild the project (you have to do this everytime you change something on the node folder):

```bash
docker-compose up
```

To connect to the database container, you have to specify the host:
```bash
mysql -u foo -h 0.0.0.0 -p
```

> **Note:** Don't forget to change the default values on the .env file ;)
