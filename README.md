### Where is docker image location in Windows 
```
%AppData%\..\Local\Docker\wsl
```

### list docker images
```
docker images
```

### build image
```
docker build -t mlr3_deploy:v1 -f dockerfile .
```

### Run container
```
docker run --rm -p 1030:1030 mlr3_deploy:v1
```
### Stop all running containers use:
```
docker stop $(docker ps -a -q)
```
### Remove image
```
docker rmi 00a21 -f
docker image rm mlr3_deploy:v1
```
