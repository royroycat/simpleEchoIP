# Simple Echo IP by nginx and certbot

Publish a simple http service to echo the client-side ip

i.e. Visit a url and return client side ip

i.e. return X.X.X.X

It is useful when your web service need to grep client side IP or simply want to check local machine ip because of connecting to other network and see is it worked.

### Usage
`cp .env.smaple .env`

Fill in the essential info in `.env`

>CERTBOT_EMAIL=YOUR EMAIL ADDRESS
>
>DOMAIN_NAME=YOUR DOMAIN NAME (e.g. ip.example.com)

`docker-compose up`

docker-nginx-certbot docker image will help to requests SSL certificates from Let's Encrypt. 
So your simple request will protect by SSL cert from port 443.

### Credit
docker-nginx-certbot docker image :

https://github.com/JonasAlfredsson/docker-nginx-certbot

Any more flexible config can ref to above docker image / git repo.
