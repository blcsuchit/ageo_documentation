# Deployment Steps

We've made the deployment steps as simple as possible. 
The deployment will be a docker-compose stack in which all the components will auto-configure themselves.
## Architecture Diagram
<img src="\assets\architecture.png">
## Build Frontend
Build the fontend project and place the entire contents of the dist/ folder in frontend/ directory here.

## Build Docker Images
We will not ship source code to target server, 
instead only built images for security with volume bindings only for persistent storage requirements.
Use the provided script `build-images.sh`

## DNS Setup

Allocate a server with a static IP and add the DNS records as follows for the domains zone

|  Record Type |  Value |
|---|---|
|  A | static-ip of server  |

## Firewall and ports

Make sure that firewall allows open access to ports 80, 443
The steps to do this depend on the firewall in use
```
sudo iptables -P INPUT ACCEPT
sudo iptables -P OUTPUT ACCEPT
sudo iptables -P FORWARD ACCEPT
sudo iptables -F
sudo apt-get install -y iptables-persistent
```

## Install Docker
```
sudo apt-get update
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh ./get-docker.sh
sudo apt install -y docker-compose
sudo systemctl enable docker.service
sudo systemctl enable containerd.service
loginctl enable-linger $USER
```

## Docker Priviledged Ports

Make sure docker can bind to priviledged ports,
```
sudo su
echo "net.ipv4.ip_unprivileged_port_start=80" >> /etc/sysctl.conf
sysctl --system
exit
```

## Docker compose setup
Make persistent directory for database and user uploads in the host machine alongside docker-compose.yaml file.

```
mkdir letsencrypt
mkdir mongo
mkdir media
```

Create a new .env file next to docker-compose.yaml and place the following contents in it.
```
DOMAIN="staging.ageo.blackcurrantapps.com"
```

you can change the domain name to whatever you like as defined in the DNS setup

## Import containers we've built earlier
```
sudo docker load --input backend.tar
sudo docker load --input frontend.tar
```

## Start docker compose

```
sudo docker-compose up -d
```

## Stop docker compose

```
sudo docker-compose down
```