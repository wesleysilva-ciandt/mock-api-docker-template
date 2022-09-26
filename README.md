# Mock API - Docker

### Template mock API's

Template de mock para API's, com objetivo ser reutilizavel.
Usando variáveis de ambientes para facilitar mudanças de URL e PORT das API's.

[<img align="center" alt="Ruben-Python" height="30" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg"> wrubenp9](https://github.com/wrubenp9)

#### Requisitos

- Docker
  [Linux](https://docs.docker.com/desktop/install/ubuntu/)
  [Windows](https://docs.docker.com/desktop/install/windows-install/)
  <br/>
- Docker Compose
  [Linux](https://docs.docker.com/compose/install/linux/)
  Incluido na instalação do docker desktop

#### Iniciar aplicação

_O parâmetro `-d` executa o container em background_

###### Cria e inicia contêineres

```
docker-compose up -d
```

###### Para e remove contêineres

```
docker-compose down -d
```

#### Server

|     | Name API        | URL            |
| :-- | :-------------- | :------------- |
| 1   | api-one-example | localhost:3030 |
| 2   | api-two-example | localhost:5050 |

#### Arch

```
api-mock
  ├── mocks
  │   ├── api-one-example
  │   │     ├── response
  │   │     ├── DockerFile
  │   │     └── endpoints.yml
  │   │
  │   └── api-two-example
  │         ├── response
  │         ├── DockerFile
  │         └── endpoints.yml
  │
  ├── .env
  ├── docker-compose.yml
  └── README.md
```

#### References

https://github.com/mrak/stubby4node
