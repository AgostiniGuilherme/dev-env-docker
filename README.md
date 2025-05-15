# Ambiente de Desenvolvimento com Docker

Este repositório fornece um ambiente de desenvolvimento portátil usando Docker para Node.js, React e Python.

## Como usar

1. Clone o repositório:
```bash
git clone https://github.com/AgostiniGuilherme/dev-env.git
cd dev-env
```

2. Suba os contêineres:
```bash
docker compose up -d
```

3. Acesse o contêiner desejado:
```bash
docker compose exec node bash
docker compose exec frontend bash
docker compose exec python bash
```

Agora você pode desenvolver livremente em qualquer máquina com Docker instalado.


# Ambiente de Desenvolvimento com Docker

Este repositório fornece um ambiente de desenvolvimento completo e portátil usando Docker, com suporte a **Node.js**, **React** e **Python**, pronto para rodar em qualquer máquina — mesmo que não tenha dependências de desenvolvimento instaladas.

## 🔧 Tecnologias disponíveis

- ✅ Node.js 18
- ✅ Python 3.10
- ✅ React (via Vite)
- ✅ Hot reload (frontend)
- ✅ Ambiente isolado via Docker Compose

---

## 🚀 Como usar

> Pré-requisitos: [Docker Desktop](https://www.docker.com/products/docker-desktop/) instalado e em execução (modo Linux no Windows).

1. Clone o repositório:
```bash
git clone https://github.com/AgostiniGuilherme/dev-env-docker.git
cd dev-env
```

2. Inicie os contêineres:
```bash
docker compose up -d
```

3. Acesse o contêiner desejado:
```bash
docker compose exec node bash         # Terminal Node.js
docker compose exec frontend bash     # Terminal Frontend (React)
docker compose exec python bash       # Terminal Python
```

---


## 📁 Estrutura

```
fullstack-dev-env/
├── frontend/           # Projeto React (Vite)
├── docker-compose.yml  # Orquestra os serviços
├── node.Dockerfile     # Container Node.js
├── python.Dockerfile   # Container Python
└── README.md
```

---

## 💡 Dicas

- Use esse repositório como **base para novos projetos**.
- Ao criar algo novo, desenvolva dentro de um dos contêineres e salve os arquivos no volume compartilhado.
- Quer instalar algo via `npm`, `pip` ou `apt`? Basta editar os Dockerfiles ou usar `docker compose exec`.

---

## ✨ Créditos

Este projeto foi idealizado e desenvolvido por **Guilherme Agostini** para possibilitar um ambiente de desenvolvimento completo, portátil e independente de configurações locais. Uma solução simples, poderosa e prática para codar de qualquer lugar.

