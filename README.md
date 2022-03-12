# Crear un ambiente de desarrollo con Docker y Python

Tutorial YouTube(https://www.youtube.com/watch?v=BvvH3ohis6E&ab_channel=DATACLOUDER)

## Construir la Imagen

docker build -t simple_app .

## Correr la imagen en Unix

docker run -it -p 8000:8000 -v $PWD:/usr/src/app simple_app

## Correr la imagen en Windows

docker run -it -p 8000:8000 -v %cd%:/usr/src/app simple_app

## Ver todos los conetenedores construidos

docker ps -a

## Ejecutar conteneder existente (construida)

docker start -a CONTAINER_ID