docker-transmission
===================

Transmission Daemon Docker Container

Don't forget to specify a password for `iaga` account and local directories:

```
    docker run -d --name transmission \
    -p 12345:12345 -p 12345:12345/udp -p 9091:9091 \
    -e ADMIN_PASS=password \
    -v /local/dir/downloads:/var/lib/transmission-daemon/downloads \
    -v /local/dir/incomplete:/var/lib/transmission-daemon/incomplete \
    iaga/transmission
```
