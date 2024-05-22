### Caddy


1. Create caddy directory and go inside it

```
mkdir -p /home/devadmin/caddy && cd /home/devadmin/caddy 
```

2. Create docker-compose.yml
 
```
nano docker-compose.yml
```
 
3. Create caddy.yaml inside caddy directory
 
```
 nano caddy.yaml
```

Edit the caddy.yaml file
--> domain name (automate)
--> Server Name Indication (SNI)
--> upstreams (put the Ip of both the server)

4. Pull the image 

```
docker-compose pull
```


5. Start the container

```
docker-compose up -d
```
