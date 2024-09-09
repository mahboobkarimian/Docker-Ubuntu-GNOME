# Docker-Ubuntu-GNOME
Full latest ubuntu desktop with GUI running on docker

## Build
`docker build -t ubuntudesktop .`

## Run
`docker run -it --rm -p 3389:3389 ubuntudesktop`

or have audio, tun and hosts's /tmp mounted:

`docker run -it -v /run/user/1000/pipewire-0:/tmp/pipewire-0 -v /tmp/:/tmp -e XDG_RUNTIME_DIR=/tmp --privileged --cap-add=NET_ADMIN --device /dev/net/tun -p 3389:3389 ubuntudesktop`

## Use
Start Remmina or any other remote desktop app, and use RDP to connect `localhost:3389` with user `user1` and password `user1`

### Set resolution
If you add a profile in Remmina, you can set the resolution.

## Firefox
Latest version of firefox will be downloaded into home directory