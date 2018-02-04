# docker-unifi-video

Docker image for the [Unifi Video controller software](https://www.ubnt.com/download/unifi-video/default/default/unifi-video-390-ubuntu-1604-x64).

Inpired by/based on the following images:

- https://github.com/pducharme/UniFi-Video-Controller
- https://github.com/exsilium/docker-unifi-video
- https://github.com/ctindel/ubiquiti-docker/tree/master/unifi-video

## Building the image

```sh
docker build . -t hedlund/unifi-video
```

## Running the image

You can simply run the included `docker-compose.yml` as an example:

```sh
docker-compose up -d
```

Then you access the Unifi Video wizard at [http://localhost:7080/](http://localhost:7080/), or `http://<ip.address>:7080/` if you're not running on a local machine.

You also probably want to update the volume mounts in the compose file.