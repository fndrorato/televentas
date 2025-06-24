# 📞 Televentas

Sistema completo com **frontend em React**, **backend em Node.js com Sequelize**, **PostgreSQL** e **Redis** — tudo orquestrado com **Docker e Docker Compose**.  
O projeto permite rápida instalação e execução de um ambiente moderno e escalável para operações de televendas.

---

## 📁 Estrutura do Projeto

```
televentas/
├── docker-compose.yml
├── frontend/
│   ├── Dockerfile
│   ├── .env.example
│   └── src/
├── backend/
│   ├── Dockerfile
│   ├── .env.example
│   └── src/
```

---

## 🛠️ Pré-requisitos

- [Docker](https://www.docker.com/)
- [Docker Compose](https://docs.docker.com/compose/)

---

## 🚀 Como instalar e rodar

1. **Clone o repositório**

```bash
git clone https://github.com/seu-usuario/televentas.git
cd televentas
```

2. **Configure os arquivos de ambiente**

```bash
cp frontend/.env.example frontend/.env
cp backend/.env.example backend/.env
```

3. **Execute os containers**

```bash
docker-compose up --build
```

4. **Acesse a aplicação**

- 🖥️ **Frontend**: [http://localhost:3000](http://localhost:3000)
- 🔌 **Backend (API)**: [http://localhost:8081](http://localhost:8081)

---

## 🧪 Comandos úteis

### Rodar migrações e seeds manualmente:

```bash
docker-compose exec backend ./entrypoint.sh
```

O script `entrypoint.sh` permite interativamente rodar as **migrations** e/ou **seeds** conforme necessidade.

---

## ⚙️ Variáveis de Ambiente

### 📁 `frontend/.env.example`

```env
REACT_APP_BACKEND_URL=http://localhost:8081
REACT_APP_HOURS_CLOSE_TICKETS_AUTO=24
```

### 📁 `backend/.env.example`

```env
NODE_ENV=production
PORT=8081

DB_HOST=db
DB_DIALECT=postgres
DB_USER=boxuser
DB_PASS=1234
DB_NAME=whats
DB_PORT=5432

REDIS_URI=redis://redis:6379
REDIS_OPT_LIMITER_MAX=1
REGIS_OPT_LIMITER_DURATION=3000
```

---

## 📦 Tecnologias utilizadas

- ⚛️ React
- 🟩 Node.js
- 🔗 Sequelize ORM
- 🐘 PostgreSQL
- 🟥 Redis
- 🐳 Docker / Docker Compose
- 🌐 Nginx (para servir o frontend em produção)

---

## 📄 Licença

Este projeto está licenciado sob os termos da [MIT License](LICENSE) ou conforme aplicável.