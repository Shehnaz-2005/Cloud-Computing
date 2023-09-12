# Docker
## Commands used to create containers on docker:-
### Pull Images:
```
docker pull hello-world
```
```
docker pull nginx
```
```
docker pull httpd
```
### See Images:
```
docker images
```
### List of Containers:
```
docker ps
```
### Port Forwarding:
```
docker run --name mynginx -p 80:80 -d nginx
docker run --name hello-world -p 80:80 -d hello-world
```
```
```
### Stop Container:
```
Docker stop nginx
```
```
Docker stop apache
```
### Remove Container:
```
Docker rm nginx
```
```
Docker rm apache
```
### Kill Container:
```
docker kill nginx
```
```
docker kill apache
```
