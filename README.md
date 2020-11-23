
## Mi primera imagen de Docker
```sh
docker pull ubuntu
docker pull alpine
```
```sh
docker run -itd ubuntu
```
```sh
docker run -itd alpine 
```

## Proxy

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

## Sitio web estático con docker

```sh
docker run -it --rm -d -p 9090:80 --name web -v $(pwd):/usr/share/nginx/html nginx
```

## Ciencia de datos

```sh
docker run -it -p 8888:8888  uracilo/bigdataben:2
```
## Funbox
```sh
docker run --rm -it wernight/funbox nyancat
```
## Otras utilidades
```sh
docker stats
```
