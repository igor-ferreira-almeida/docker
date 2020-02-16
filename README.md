# Docker

## 1. Uso básico do Docker

### 1.1 Baixar uma imagem do repositório do Docker (Docker Hub)

```
docker image pull NOME_IMAGE

Exemplo: docker image pull hello-world
```

Também é possível baixar uma versão específica:

```
docker pull IMAGEM:VERSÃO

Exemplo: docker pull ubuntu:14.04
```

Para visualizar as imagens baixadas para o seu repositório local utilize o seguinte comando:

```
docker images
```

### 1.2 Criar um container 

O comando para criar um novo container recebe como base, podem existir muitos containers baseados em uma única imagem, uma boa analogia seria que a imagem é um projeto e o container é um objeto criado a partir deste projeto.

```
docker container create NOME_IMAGE

Exemplo: docker container create ubuntu
```

Ao executar esse comando é mostrado o **ID do container** (gerado automaticamente) logo em seguida

É possível dar um nome a este container no momento da criação dele:

```
docker container create --name "NOME_DO_CONTAINER" NOME_DA_IMAGEM

Exemplo: docker container create --name "mizar" hello-world
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

Exemplo: docker run hello-world
```
