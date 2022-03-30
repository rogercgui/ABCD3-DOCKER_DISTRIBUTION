# ABCD3-DOCKER\_DISTRIBUTION

Docker-compose configuration to deploy ABCD 3.0 using Docker containers

# ABCD3

## Installing on Ubuntu

### Install cURL

Update your Ubuntu:

```
sudo apt update && sudo apt upgrade
```

Next, install cURL, execute:

```
sudo apt install curl
```

Verify install of curl on Ubuntu by running:

```
curl --version
```

Search for libcurl bindings for your programming needs:

```
apt-cache search libcurl | grep python
```

Install the Python bindings to libcurl:

```
sudo apt install python3-pycurl
```

Search for other curl bindings to libcurl:

```
apt-cache search libcurl
```

### Install Docker

Command:

```
sudo apt install docker
```

Run this command to download the current stable release of Docker Compose:

```
sudo curl -L "https://github.com/docker/compose/releases/download/1.25.5/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```

Next:

```
sudo apt-get install docker.io docker-compose docker-doc
```

### Start docker

```
sudo systemctl start docker.service
```

```
sudo systemctl enable docker.service
```

Verify version:

```
docker-compose --version
```

Clone the repository:

```
gh repo clone ABCD-DEVCOM/ABCD3-DOCKER_DISTRIBUTION
```

or download the zip and unzip the package [Here](https://github.com/ABCD-DEVCOM/ABCD3-DOCKER_DISTRIBUTION/archive/refs/heads/main.zip)

Inside the repository folder type:

```
sudo docker-compose -f docker-compose.yaml up -d	
```

### Access

Access in your browser the address: http://localhost:5800

User: superadmin

Password: abcd
