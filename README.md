# 🐇 Mensageria com FastAPI + RabbitMQ (Docker Compose)

Projeto desenvolvido para demonstrar comunicação entre uma API FastAPI e um sistema de mensageria **RabbitMQ** utilizando **Docker Compose**.

---

## 🚀 Tecnologias
- FastAPI
- RabbitMQ
- Docker / Docker Compose
- Python 3.12
- Pika (cliente AMQP)

---

## 🧩 Estrutura dos Serviços

| Serviço | Função |
|----------|--------|
| **api** | Recebe requisições REST e envia mensagens à fila RabbitMQ |
| **consumer** | Lê e imprime mensagens da fila |
| **rabbitmq** | Sistema de mensageria com painel em `http://localhost:15672` |

---

## ⚙️ Como rodar o projeto

### 1️⃣ Subir os containers
```bash
docker compose up --build

Acesse: http://localhost:15672

Login: appuser
Senha: apppass
