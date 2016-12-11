# gxro
## rproxy

apache reverse proxy.
+ `auth` Basic auth
+ `cert` site-ssl.key, site-ssl.crt, ca.crt
+ `conf.d` `/etc/apache2/conf.d` Apache Config Files

## apt.sra.gx

rproxy + apt cacher ng
+ `cache` apt cache dir

## hub.sra.gx

rproxy + apt cacher ng + docker registry + utils(openssl,htpasswd)
+ `registry` docker image registry

```
docker-compose exec auth-utils bash
```

## redmine.sra.gx + mysql.sra.gx
