# bepasty-docker

Docker automated build repository for the [bepasty server](https://github.com/bepasty/bepasty-server)

## Usage

Install docker on your system. for the restart feature you need at least docker 1.2.
[Instructions](http://docs.docker.com/installation/)


_First start/"setup"_

This fetches the image (if you haven't already done that)
```
docker run --restart=always --name bepasty -p 5000:5000 -v /opt/bepasty:/srv/bepasty asmaps/bepasty
```

_Stop the server_

```
docker stop bepasty
```

_Start the server_

With the --restart=always option the server should be started automatically. If you stopped it you can start it again by
running
```
docker start bepasty
```
