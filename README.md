# 📞 Televentas

Sistema completo com **frontend em React**, **backend em Node.js com Sequelize**, **PostgreSQL** e **Redis** — tudo orquestrado com Docker.

---

## 📁 Estrutura do Projeto

televentas/
├── docker-compose.yml
├── frontend/
│ ├── Dockerfile
│ ├── .env.example
│ └── src/
├── backend/
│ ├── Dockerfile
│ ├── .env.example
│ └── src/


---

## 🛠️ Pré-requisitos

- Docker
- Docker Compose

---

## 🚀 Como instalar e rodar

1. **Clone o repositório**

```bash
git clone https://github.com/seu-usuario/televentas.git
cd televentas

2. **Execute os containers**
```bash
docker-compose up --build

3. **Acesse a aplicação**
- Frontend: http://localhost:3000
- Backend (API): http://localhost:8081

📦 Tecnologias utilizadas

React
Node.js
Sequelize ORM
PostgreSQL
Redis
Docker / Docker Compose
Nginx (para servir o frontend em produção)