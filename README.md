# dokku minio (beta)
Official mongo plugin for dokku. Currently defaults to installing [latest](https://hub.docker.com/r/minio/minio/).

## requirements

- dokku 0.4.0+
- docker 1.8.x

## installation

```shell
# on 0.3.x
cd /var/lib/dokku/plugins
git clone https://github.com/dokku/dokku-mongo.git mongo
dokku plugins-install

# on 0.4.x
dokku plugin:install https://github.com/dokku/dokku-mongo.git mongo
```

## commands

```
minio:clone <name> <new-name>  Create container <new-name> then copy data from <name> into <new-name>
minio:connect <name>           Connect via telnet to a minio service
minio:create <name>            Create a minio service with environment variables
minio:destroy <name>           Delete the service and stop its container if there are no links left
minio:info <name>              Print the connection information
minio:link <name> <app>        Link the minio service to the app
minio:list                     List all minio services
minio:logs <name> [-t]         Print the most recent log(s) for this service
minio:promote <name> <app>     Promote service <name> as MONGO_URL in <app>
minio:restart <name>           Graceful shutdown and restart of the minio service container
minio:start <name>             Start a previously stopped minio service
minio:stop <name>              Stop a running minio service
minio:unlink <name> <app>      Unlink the minio service from the app
```

## usage
TODO: 書く
