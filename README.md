# docsify-starter

> A Docsify starter, with local PlantUML server

This repo just sets up a basic docsify environment:

* [Docker Compose](https://docs.docker.com/compose/) to setup and run:
  * [A Docsify container](https://docsify.js.org/), listening on Port 10000
  * [A local PlantUML server](https://plantuml.com/), listening on Port 10001

## Use docker-compose

To get started quickly, just do:

```
$ git clone https://github.com/bylexus/docsify-starter.git
$ cd docsify-starter
$ docker-compose up
```

There are now 2 containers running:

* `docsify`: Docsify on Port 10000 (So browse to http://localhost:10000)
* `plantuml`: PlantUML server on Port 10001 ( generate PlantUML on the fly: http://localhost:10001/png/SyfFKj2rKt3CoKnELR1Io4ZDoSa70000)

Feel free to adapt the `docker-compose.yml` file as needed!

If you need to interact with `docsify-cli`, do so through docker:

```
$ docker exec -ti docsify docsify help
```

Your docsify docs are in the `docs/` dir. Feel free to edit them as needed!

## Note for git users

This Repo is meant as template. After cloning, feel free to delete the `.git` dir, and init your own git, e.g.:

```
$ git clone https://github.com/bylexus/docsify-starter.git
$ cd docsify-starter
$ rm -rf .git
$ git init
```
