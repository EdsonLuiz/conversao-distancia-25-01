# conversao-distancia

## Execução em ambiente local

Construir a imagem
```shell
docker build -t conversao-distancia -f Dockerfile .
```

Inicializar aplicativo através da imagem gerada localmente.
```shell
docker container run -d --rm --name conversao-distancia -p 5000:5000 conversao-distancia
```

## Execução dockerhub

Inicializar aplicativo através da imagem hospedada no dockerhub.
```shell
docker container run -d --rm --name conversao -p 5000:5000 edsonluiz/conversao-distancia:v1
```