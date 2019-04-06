# https-docker-apache
Docker Apache container with https turned after inserting certs

## Sertificates

### Create self-signes certificates using OpenSSL 
#### This will create certificate and key
```
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout server.key -out server.crt
```

### Get certificate from Let’s Encrypt(https://letsencrypt.org/) using Certbot(https://certbot.eff.org/)
#### Install Cerbot and follow instructions and you should end up with certificate file and key
```
sudo yum install certbot
sudo certbot certonly
```


