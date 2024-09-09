# Docker-Ubuntu-GNOME
Full ubuntu desktop with GUI running on docker

## Build
`docker build -t ubuntudesktop .`

## Run
`docker run -it --rm -p 3389:3389 ubuntudesktop`

## Use
Start Remmina or any other remote desktop app, and use RDP to connect `localhost:3389` with user and password both `ubuntu`

### Set resolution
If you add a profile in Remmina, you can set the resolution.
