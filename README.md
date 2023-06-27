# Projeto Docker-FullStack

Este é o README.md para o projeto Docker-FullStack.

## Universidade Federal do Amazonas - Instituto de Computação (ICOMP)

Web Academy - Capacitação e Desenvolvimento em Web Full Stack
Trabalho Prático - Docker
Aluno: Gleides Vinente

### Objetivo

O objetivo deste trabalho prático é colocarmos em prática os conceitos aprendidos durante o módulo de Docker, colocando uma aplicação web no ar utilizando contêineres.

## Descrição

Você foi responsável por colocar no ar a aplicação de listagem de livros do Web Academy. Foi sugerido que a aplicação funcionasse de maneira flexível e de fácil configuração entre ambientes, então você decidiu utilizar o Docker para rodar as aplicações.

A infraestrutura dessa aplicação consiste em:

- Um servidor de banco de dados MySQL
- Uma aplicação backend escrita em Node.js com Typescript
- Uma aplicação frontend escrita em React com Typescript
- Uma aplicação de gerenciamento de banco de dados, o PHPMyAdmin

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
