
## Mi primera imagen de Docker
```sh
docker run -itd ubuntu
```

```sh
docker run -itd alpine 
```

## Sitio web estatico con docker

```sh
docker pull nginx 
```

```sh
docker run -it --name=web
```

```sh
docker exec -it web ls /usr/share/nginx/html
```
```sh
docker exec -it web cat /usr/share/nginx/html/index.html
```
```sh
docker run -it --rm -d -p 8080:80 --name web -v $(pwd):/usr/share/nginx/html nginx
```
```sh
docker stats
```
