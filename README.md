# prism-to-k8s
Run in Docker Desktop

## Check compose
```
$kubectl api-versions | grep compose
compose.docker.com/v1beta1
compose.docker.com/v1beta2
```

## Run Stack
```
docker stack deploy --orchestrator=kubernetes -c docker-compose.yml demo01
```

## Delete Stack
```
kubectl delete stack demo01
```

## Reference
http://www.somkiat.cc/docker-compose-on-kubernetes/

https://www.docker.com/blog/simplifying-kubernetes-with-docker-compose-and-friends/