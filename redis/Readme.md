### Redis 
#### folder architecture




| port | component | 
| -------- | -------- | 
| 6379     | redis     | 



1.  Create redis directory and go inside it
```
mkdir -p /home/devadmin/redis && cd /home/devadmin/redis 
```

2. Redis docker-compose.yml

```
nano docker-compose.yml
```

3. redis.conf
```
nano redis.conf
```

4. Give permission to logs folder
```
chmod 777 logs
```

5. Pull the image and start the container
```
docker-compose pull
```
```
docker-compose up -d
```
