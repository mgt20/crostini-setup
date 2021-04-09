#docker-crostini-setup

Sets up Docker, docker-compose, and required permissions inside of the default Crostini (Debian) container on CrOS

## Pre-requisites
- Crostini must be installed and running on the CrOS device
- All commands below must be entered into the Crostini container that runs Debian: the Hostname is "Penguin" by default. Launch the "Terminal" app on CrOS to enter the bash shell for this container.

## How-To
1. Create a directory, clone the repo, and make the script executable:

```
mkdir ~/github && cd ~/github
git clone https://github.com/mgt20/docker-crostini-setup.git
cd docker-crostini-setup
chmod +x docker-crostini-setup.sh
```

2. Execute the script:

```
cd ~/github/docker-crostini-setup/
./docker-crostini-setup.sh
```

3. Test Docker by running:

```
docker run hello-world
```
