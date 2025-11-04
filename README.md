# Ambiente Docker Compose Flask + MySQL

Este projeto cria um ambiente completo utilizando **Docker Compose** para rodar uma aplicação **Flask (Python)** integrada a um banco de dados **MySQL**.

---

## Estrutura do projeto

```
meu-compose-lab/
├── app.py                # Código principal do servidor Flask
├── Dockerfile            # Define a imagem da aplicação Flask
├── docker-compose.yml    # Define os serviços (Flask + MySQL)
└── README.md             # Documentação do projeto
```


## Como funciona

* O **Docker Compose** cria dois containers:

  1. **flask_app** → executa o servidor Flask.
  2. **mysql_db** → executa o banco de dados MySQL.
* O Flask se conecta ao banco usando as variáveis de ambiente definidas no `docker-compose.yml`.

---

## Testando a conexão

A rota principal `/` tenta conectar ao banco MySQL e retorna:

* **Conexão OK!** — se a conexão foi bem-sucedida
* **Erro ao conectar** — se houve algum problema (mensagem exibida na página)



