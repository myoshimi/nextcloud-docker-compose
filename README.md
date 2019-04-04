# nextcloud-docker-compose

====

Nextcloud with HTTPS reverse proxy by docker-compose.yml.

# Prerequirements

* Prepare two key files shown below to provide HTTPS connection.
    * SSL Certificate file (e.g. fullchain.pem)
    * SSL Certificate key file (e.g. privkey.pem)
    * Typically, these files can be obtained by ```certbot``` command which gets certificate by let's encrypt.

# Usage

```
git clone https://github.com/myoshimi/nextcloud-docker-compose
cd nextcloud-docker-compose
cp <Directory Path>/fullchain.pem ./keys/
cp <Directory Path>/privkey.pem ./keys/
docker-compose up -d
```

