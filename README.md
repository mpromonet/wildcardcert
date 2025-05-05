test wildcard certificate
---

```
docker compose up

# with curl
curl https://toto.dev.localhost/ -v --cacert certs/server.crt 
curl https://titi.dev.localhost/ -v --cacert certs/server.crt 

# with wget
wget https://anything.dev.localhost/ --verbose --ca-certificate=./certs/server.crt -O -
```