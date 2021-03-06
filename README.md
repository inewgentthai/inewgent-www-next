Horeca Next JS Template
======

NOTE
----
The master branch will always contain the latest stable version. If you wish to check older versions or newer ones currently under development, please switch to the relevant branch.

Get Started
-----------

#### Requirements

To run this application on your machine, you need at least:

* docker-compose
* >= Node.js 12.13.1
* Nextjs >= 9.4.2


Application flow pattern:
---------------------
http://git365.eggdigital.com/horeca/horeca-next-template.git

Run the docker for development:
---------------------
First you need to copy `.env.example` to `.env` for setup environment of appplication

You can now build, create, start, and attach to containers to the environment for your application. To build the containers use following command inside the project root:

```bash
docker-compose build
```

To start the application and run the containers in the background, use following command inside project root:

```bash
docker-compose up -d
docker exec -u root -it horeca-next-template chown -R www-data:www-data /var/www/html
```
```bash
docker-compose down
```

Installing Dependencies via Composer
------------------------------------
Run the composer installer:

```bash
docker exec -it horeca-next-template nmp install
```
or
```bash
docker exec -it horeca-next-template npm update
```

Map the domain
------------------------------------
Open the hosts file on your local machine `/etc/hosts`.
```bash
127.0.0.1  next-template.eggsmartpos.local
```

Running Application
------------------------------------
Open the browser
```bash
http://next-template.eggsmartpos.local:5002
```

# inewgent-www
