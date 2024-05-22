1. Create sentinel directory and go inside it

```
mkdir -p /home/devadmin/sentinel && cd /home/devadmin/sentinel
```

2. Create docker-compose.yml file

```
nano docker-compose.yml
```

3. Create a sentinel.conf file inside conf 
 
```
nano /home/devadmin/sentinel/conf/sentinel.conf 
```

4. Pull the image and start the container

```
docker-compose pull
```
```
docker-compose up -d
```
