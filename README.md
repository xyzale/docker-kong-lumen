# Kong + Lumen on Docker

This docker-compose file will run the needed containers to let Kong run properly and a container with a Lumen application. 

## What is Kong?

You can find the official Docker distribution for Kong at [https://hub.docker.com/r/mashape/kong/](https://hub.docker.com/r/mashape/kong/)

### How to use
To run this template execute:

```shell
$ docker-compose up
```

### Lumen app

The application is not included with this repository.

You should map your Lumen application folder in the `docker-compose.yml` file under the lumen container configuration.

Lumen app is reachable through the poert 8123, so on Kong you should map the upstream_url as the docker container ip with the 8123 port. Edit the docker-compose.yml if you're not happy with it.


