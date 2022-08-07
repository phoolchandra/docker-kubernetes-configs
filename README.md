# docker-kubernetes-configs

## Docker commands
```
$ docker ps 
$ docker inspect 35418a760e02 | grep "IPAddress"
$ docker-compose -f docker-compose.yaml up -d
$ docker compose up
```


## kafka-connect set up
docker command to up the landoop/Kafka-connect UI <br>
```
$ docker run --rm -it -p 8000:8000 \
	           -e "CONNECT_URL=http://ip:28083;kafka-connect-1,http://ip;kafka-connect-2" \
	           -e "PRPXY=false" \
	           landoop/kafka-connect-ui
```

> http://ip;kafka-connect-1: first part is cluster ip address and second part is clustername

Usefull link for kafka-connect
1. https://hub.docker.com/r/landoop/kafka-connect-ui
2. https://github.com/lensesio/kafka-connect-ui
