# Ambiente de Desenvolvimento Portátil com Docker

Este repositório ambiente de desenvolvimento full stack portátil com Docker, pronto para rodar Node.js, React e Python de qualquer lugar. 

Ideal para testes, protótipos e desenvolvimento em máquinas sem dependências instaladas.


## 🔧 Tecnologias disponíveis

- ✅ Node.js 18
- ✅ Python 3.10
- ✅ React (via Vite)
- ✅ Hot reload (frontend)
- ✅ Ambiente isolado via Docker Compose

---


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
docker compose exec node bash         # Terminal Node.js
docker compose exec frontend bash     # Terminal React (frontend)
docker compose exec python bash       # Terminal Python
```

Agora você pode desenvolver livremente em qualquer máquina com Docker instalado.

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

Este projeto foi idealizado e desenvolvido por **Guilherme Agostini** para oferecer um ambiente de desenvolvimento completo, portátil e independente de configurações locais. Uma solução simples, prática e poederosa para codar de qualquer lugar.

