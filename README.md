# 🔐 Password Manager API


### *(English version below / versão em português abaixo)*  

---

## 🇧🇷 Português

Um **gerenciador de senhas seguro** com API em **Python + FastAPI**, utilizando **hash Argon2 com salt aleatório** e autenticação via **JWT**.  
Este projeto é focado em estudo e demonstração de **boas práticas de backend seguro**.  

---

### 🚀 Tecnologias
<p align="left">
  <!-- Python -->
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white" alt="Python" />
  
  <!-- FastAPI -->
  <img src="https://img.shields.io/badge/FastAPI-0.95+-009688?logo=fastapi&logoColor=white" alt="FastAPI" />
  
  <!-- SQLAlchemy + SQLite/Postgres -->
  <img src="https://img.shields.io/badge/SQLAlchemy-red?logo=databricks&logoColor=white" alt="SQLAlchemy" />
  <img src="https://img.shields.io/badge/SQLite-07405e?logo=sqlite&logoColor=white" alt="SQLite" />
  
  <!-- Passlib -->
  <img src="https://img.shields.io/badge/Passlib-Argon2-green" alt="Passlib Argon2" />
  
  <!-- PyJWT -->
  <img src="https://img.shields.io/badge/PyJWT-Auth-orange" alt="PyJWT" />
  
  <!-- Docker -->
  <img src="https://img.shields.io/badge/Docker-blue?logo=docker&logoColor=white" alt="Docker" />
</p>

---
### 📂 Estrutura do Projeto (Português)

### 📂 Estrutura do Projeto
```bash

password-manager-api/
│── app/
│   ├── app.py          # ponto de entrada da aplicação
│   ├── core/            # configs, segurança, dependências
│   ├── models/          # modelos ORM (SQLAlchemy)
│   ├── domain/          # camada de dominio, usecase etc
│   ├── routes/          # rotas (auth, users, passwords)
│   ├── utils/           # helpers (logger, gerador de salt)
│   └── db/              # conexão e migrations
│
├── tests/               # testes unitários
├── .env.example         # exemplo de variáveis de ambiente
├── requirements.txt     # dependências
├── docker-compose.yml   # (opcional) subir via docker
└── README.md            # documentação

```
### ⚙️ Como Rodar
```bash
# Clone o repositório
git clone https://github.com/seuusuario/password-manager-api.git
cd password-manager-api

# Crie e ative o ambiente virtual
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

# Instale as dependências
pip install -r requirements.txt

# Configure o arquivo .env
cp .env.example .env

# Execute a aplicação
uvicorn app.main:app --reload

```
Acesse a documentação interativa:  
👉 [http://localhost:8000/docs](http://localhost:8000/docs)

---


## 🇬🇧 English

### A secure password manager with Python + FastAPI backend, using Argon2 hashing with random salt and JWT authentication.
This project is focused on learning and demonstrating secure backend best practices.

### 🚀 Stack
<p align="left">
  <!-- Python -->
  <img src="https://img.shields.io/badge/Python-3.10+-blue?logo=python&logoColor=white" alt="Python" />
  
  <!-- FastAPI -->
  <img src="https://img.shields.io/badge/FastAPI-0.95+-009688?logo=fastapi&logoColor=white" alt="FastAPI" />
  
  <!-- SQLAlchemy + SQLite/Postgres -->
  <img src="https://img.shields.io/badge/SQLAlchemy-red?logo=databricks&logoColor=white" alt="SQLAlchemy" />
  <img src="https://img.shields.io/badge/SQLite-07405e?logo=sqlite&logoColor=white" alt="SQLite" />
  
  <!-- Passlib -->
  <img src="https://img.shields.io/badge/Passlib-Argon2-green" alt="Passlib Argon2" />
  
  <!-- PyJWT -->
  <img src="https://img.shields.io/badge/PyJWT-Auth-orange" alt="PyJWT" />
  
  <!-- Docker -->
  <img src="https://img.shields.io/badge/Docker-blue?logo=docker&logoColor=white" alt="Docker" />
</p>

### 📂 Project 
```bash
password-manager-api/
│── app/
│   ├── main.py          # application entry point
│   ├── core/            # configs, security, dependencies
│   ├── models/          # ORM models (SQLAlchemy)
│   ├── domain/          #
│   ├── routes/          # routes (auth, users, passwords)
│   ├── services/        # business logic (hash, jwt, auth)
│   ├── utils/           # helpers (logger, salt generator)
│   └── db/              # database connection and migrations
│
├── tests/               # unit tests
├── .env.example         # environment variables example
├── requirements.txt     # dependencies
├── docker-compose.yml   # (optional)
└── README.md            # documentation
```

###⚙️ How to Run
```bash
# Clone repository
git clone https://github.com/youruser/password-manager-api.git
cd password-manager-api

# Create and activate virtual environment
python -m venv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows

# Install dependencies
pip install -r requirements.txt

# Configure environment variables
cp .env.example .env

# Run the application
uvicorn app.main:app --reload

Access interactive documentation:
👉 http://localhost:8000/docs
```
## 🛡️ Segurança / Security

Senhas armazenadas com Argon2 + salt aleatório.
Autenticação via JWT.
Variáveis sensíveis isoladas em .env.

## 📌 Roadmap

API base with authentication
Argon2 + salt password hashing
User vault management
Automated tests
Docker deploy
Mobile app integration

# 📜 Licença / License

Este projeto é de uso livre para fins educacionais. 
This project is free to use for educational purposes.
