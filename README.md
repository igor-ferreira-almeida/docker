# Docker

## 1. Uso básico do Docker

### 1.1 Baixar uma imagem do repositório do Docker (Docker Hub)

```
docker image pull NOME_IMAGE

// Exemplo
docker image pull hello-world
```

Também é possível baixar uma versão específica:

```
docker pull IMAGEM:VERSÃO

// Exemplo
docker pull ubuntu:14.04
```

### 1.5 Executar os quatro comandos anteriormente apresentados

Este comando executa na verdade os seguintes outros comandos:

```
docker image pull NOME_IMAGE
docker container create NOME_CONTAINER
docker container start NOME_CONTAINER
docker container exec NOME_CONTAINER
```

```
docker run NOME_IMAGE

docker run hello-world
```
