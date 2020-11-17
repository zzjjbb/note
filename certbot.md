# Certbot & Let's Encrypt

## Setup

```sh
sudo certbot certonly --manual --preferred-challenges dns
```

## Renew

```sh
sudo certbot certonly --force-renew --manual --preferred-challenges dns
```
