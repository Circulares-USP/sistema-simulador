# Simulador de Demanda

## _Setup_

### Arquivos

Primeiro, clone o repositório com a flag `--recurse-submodules`, para que os submódulos do _front-end_ e do _back-end_ sejam integrados à raiz
desse repositório. Após isso, copie os arquivos-exemplo de variáveis de ambiente do _front-end_ e do repositório principal da aplicação,
editando-os conforme necessário:

```bash
$ cp .env.sample .env
$ cp frontend/.env.sample frontend/.env
```

O _endpoint_ do _back-end_, caso seja diferente do local utilizado pelo Docker, deve ser modificado em `frontend/.env`

### Inicialização e Desenvolvimento

O projeto utiliza o [Docker](https://docs.docker.com/engine/install/) e o plugin (Docker Compose)[https://docs.docker.com/compose/install/linux/]
para rodar. O ambiente de desenvolvimento pode ser iniciado com:

```bash
$ docker compose up [-d]
```

A _flag_ `-d` permite que os contêineres rodem em segundo plano. A aplicação principal é, por padrão, hospedada no link `http://localhost:3001`.
Para editar a porta local, basta modificar o arquivo `docker-compose.yml`.
