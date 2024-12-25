Jellyfin for private/internal use in (Bootable) Containers
==========================================================

```bash
$ podman run -d --name jellyfin --hostname ${HOSTNAME}-jellyfin --net=ncentre-bridge --ip 10.0.21.160  \
    --cap-add=NET_ADMIN --cap-add=NET_RAW --device=/dev/net/tun --cap-add=SYS_ADMIN --device=/dev/fuse \
    ghcr.io/gbraad-homelab/jellyfin:latest
```
