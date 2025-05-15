# Ambiente de Desenvolvimento com Docker

Este repositório fornece um ambiente de desenvolvimento portátil usando Docker para Node.js, React e Python.

## Como usar

1. Clone o repositório:
```bash
git clone https://github.com/seu-usuario/dev-env.git
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