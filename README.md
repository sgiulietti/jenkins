# Step by step demo complete CI/CD pipeline using Jenkins

## PREREQUISITES

Tener instalado Jenkins como un contenedor Docker en un servidor dedicado.

## Caracteristicas del servidor y detalle del sofware instalado para el demo

Servidor linux Ubuntu versión 24.10

### Commandos ejecutados 

```bash
atp update
```
### Instalar docker

```bash
apt install docker.io
```

### Instalar Jenkins container
Se abren los 2 puertos necesarios, se agrega un volume para persist data

```bash
docker run -p 8080:8080 -p 50000:50000 -d -v jenkins_home:/var/jenkins_home jenkins/jenkins:lts-jdk17
```