# docker-tomcat85-java8

Este repositorio se encarga de servir como estructura de recursos utilizados para los artículos publicados en la plataforma enmilocalfunciona.io relacionados con el uso de contenedores para acelerar los desarrollos

## Stack Tecnológico

- Java 8
- Docker - Tecnología de Contenedores/Containers
- Docker Hub - Repositorio de Docker Publico

## Prerequisitos

- Java 8 instalado (1.5+ version requerido)
- Docker instalado (19+)
- Docker-Compose

## Instalación de JAVA 8

### CENTOS 8

```bash

$ sudo yum install java-1.8.0-openjdk

$ sudo update-alternatives --config java

$ sudo echo "export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.191.b12-1.el7_6.x86_64/jre/bin/java" >> ~/.bash_profile

$ sudo source ~/.bash_profile

```

## Instalación de Docker

- Guía Oficial: https://docs.docker.com/engine/install/centos/

## Instalación Docker-Compose

```
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.28.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose

```





