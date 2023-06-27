# Projeto Docker-FullStack - README.md

Este é o README.md para o projeto Docker-FullStack.

## Repositório Remoto

O repositório remoto do projeto está disponível no GitHub.
Você pode acessá-lo em: [https://github.com/gleideveloper/Docker-FullStack](https://github.com/gleideveloper/Docker-FullStack).

## Pré-condição

Antes de executar o projeto, certifique-se de ter o Docker instalado em sua máquina.

## Estrutura de Pasta

Certifique-se de que a estrutura de pasta do projeto esteja organizada da seguinte forma:

```
Docker-FullStack/
  ├── backend/
  │   ├── ... arquivos e pastas do backend ...
  │   └── Dockerfile
  ├── frontend/
  │   ├── ... arquivos e pastas do frontend ...
  │   └── Dockerfile
  └── docker-compose.yml
```

## Comandos Docker para execução

### Rodar o projeto

```
docker-compose up -d
```

Este comando irá executar o projeto utilizando o Docker Compose, criando e iniciando os containers necessários em segundo plano (-d).

### Listar os containers

```
docker ps
```

ou

```
docker-compose ps
```

Estes comandos listarão os containers em execução.

### Listar as imagens

```
docker images
```

ou

```
docker image ls
```

Estes comandos listarão as imagens disponíveis.

### Listar os volumes

```
docker volume ls
```

Este comando listar os volumes criados pelo Docker.

### Checar local do volume do banco

- **Logs do Projeto**

```
ls -la ./webacademy-livros-backend/log
```

- **Banco de dados MySql**

```
sudo ls -la /var/lib/docker/volumes/docker-fullstack_dbMyApp/_data
```

Este comando exibirá o local do volume do banco de dados. Certifique-se de substituir "docker-fullstack_dbMyApp" pelo nome correto do volume utilizado em seu projeto.

### Listar as networks

```
docker network ls
```

Este comando listar as networks criadas pelo Docker.

Espero que essas informações sejam úteis para executar o projeto.
