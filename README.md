# crostini-setup

Sets up Docker, docker-compose, required permissions, and other config/software inside of the default Crostini (Debian) container on CrOS

## Pre-requisites
- Crostini must be installed and running on the CrOS device
- All commands below must be entered into the Crostini container that runs Debian: the Hostname is "Penguin" by default. Launch the "Terminal" app on CrOS to enter the bash shell for this container.

## How-To
1. Download the script and run it:

```
curl -o- https://raw.githubusercontent.com/mgt20/crostini-setup/main/script.sh | bash
```

2. Reboot, log in/out, or run this command to make the group changes take affect:

```
newgrp docker
```

3. Test Docker by running:

```
docker run hello-world
```
