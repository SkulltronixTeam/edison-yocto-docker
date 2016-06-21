# edison-yocto-docker

## create a suitable docker machine

```
docker-machine create --driver virtualbox --virtualbox-disk-size "131072" --virtualbox-memory "4096" edison
eval $(docker-machine env edison)
```

## build image

```
git clone git@github.com:SkulltronixTeam/edison-yocto-docker.git
cd edison-yocto-docker
./build
```

Get comfortable, this will take hours :-) (6/21/2016)
