### Crear imagen y ejecutar un contenedor

`docker build -f docker/Dockerfile -t docker-php .`

`docker run --rm -p 80:80 docker-php`