## SETTING WITH NGINX, GUNICORN


### How to get a certificate


#### Install certbot

```
$ sudo add-apt-repository ppa:certbot/certbot
$ sudo apt-get update
$ sudo apt-get install python-certbot-nginx
```


#### Get certificate

```
sudo certbot certonly --manual --preferred-challenges dns --server https://acme-v02.api.letsencrypt.org/directory -d 'stockin.kr'
```


#### Set DNS txt record
###### host : "\_acme-challenge", value: key in certbot


