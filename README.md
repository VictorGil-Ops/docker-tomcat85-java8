# docker-tomcat85-java8

Este repositorio sirve para instalar un contedor docker tomcat 8.5 y la versión de java 8.

## Stack Tecnológico

- Java 8
- Docker - Tecnología de Contenedores/Containers
- Docker Hub - Repositorio de Docker Publico

## Prerequisitos

- Java 8 instalado (1.5+ version requerido)
- Docker instalado (19+)
- Docker-Compose (1.28+)

## Instalación en CENTOS 8

### Instalación de JAVA 8

```bash
$ sudo yum install java-1.8.0-openjdk
$ sudo update-alternatives --config java
$ sudo echo "export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.191.b12-1.el7_6.x86_64/jre/bin/java" >> ~/.bash_profile
$ sudo source ~/.bash_profile
```

### Instalación de Docker

- Guía Oficial: https://docs.docker.com/engine/install/centos/

### Instalación Docker-Compose

```bash
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.28.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```

### Lanzar contendor con docker-compose

Desde la ubicación de docker-compose.yaml

```bash
$ docker-compose up --build -d
``` 

## Instalación en UBUNTU 18

### Instalación de JAVA 8

```bash
$ sudo apt update
$ sudo apt install openjdk-8-jdk openjdk-8-jre
$ cat >> /etc/environment <<EOL
JAVA_HOME=/usr/lib/jvm/java-8-openjdk-amd64
JRE_HOME=/usr/lib/jvm/java-8-openjdk-amd64/jre
EOL
```

### Instalación de Docker

- Guía Oficial: https://docs.docker.com/engine/install/ubuntu/

### Instalación Docker-Compose

```bash
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.28.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
```

### Lanzar contendor con docker-compose

Desde la ubicación de docker-compose.yaml

```bash
$ docker-compose up --build -d
``` 
